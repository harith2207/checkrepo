pipeline {

  agent any

  options {

    buildDiscarder logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '5', daysToKeepStr: '', numToKeepStr: '5')

  }

 stage ('Call Powershell Script')
{
    node ('MyWindowsSlave') {
        PowerShell(". '.\\disk-usage.ps1'") 
    }
}
}

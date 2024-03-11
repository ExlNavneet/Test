pipeline {
  agent any
environment {

SITEBASEURL = null
APIKEY = null
PACKAGEFILENAME = null
initiateInspectionJson = null
deploymentResponseJson = null
response = null
warnings = null
errors = null
DEPLOYMENTNAME = null
DEPLOYMENTDESCRIPTION = null
}
  stages {
    
    
    stage("Perpare ADM") {
      steps {
        script {
          //def jenkinsUtils = load "groovy/JenkinsUtils.groovy"

          // Setup ADM
          bat "C:\ProgramData\Jenkins\.jenkins\workspace\Test2\devops>tar -xf adm.zip"
          bat "tar -xf C:\ProgramData\Jenkins\.jenkins\workspace\Test2\devops\adm>tar -xf automated-versioning-manager-(avm)-2.5.30.zip"
		  bat "tar -xf C:\ProgramData\Jenkins\.jenkins\workspace\Test2\devops\adm>tar -xf automated-import-manager-(aim)-client-2.5.27.zip"
          //jenkinsUtils.setProperty("adm/appian-version-client/metrics.properties", "pipelineUsage", "true")
		  //jenkinsUtils.setProperty("adm/appian-import-client/metrics.properties", "pipelineUsage", "true")
          
        }
      }
    }
    
    
  }
}



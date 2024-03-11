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
          sh "unzip devops/adm.zip -d adm"
          sh "unzip adm/automated-versioning-manager-(avm)-2.5.30.zip -d adm/appian-version-client"
		  sh "unzip adm/automated-import-manager-(aim)-client-2.5.27.zip -d adm/appian-import-client"
          //jenkinsUtils.setProperty("adm/appian-version-client/metrics.properties", "pipelineUsage", "true")
		  //jenkinsUtils.setProperty("adm/appian-import-client/metrics.properties", "pipelineUsage", "true")
          
        }
      }
    }
    
    
  }
}



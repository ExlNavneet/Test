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
          def jenkinsUtils = load "groovy/JenkinsUtils.groovy"

          // Setup ADM
          sh "unzip devops/Test.zip -d admTest"
          sh "unzip admTest/automated-versioning-manager-(avm)-2.5.30.zip -d admTest/appian-version-client"
		  sh "unzip admTest/automated-import-manager-(aim)-client-2.5.27.zip -d admTest/appian-import-client"
          jenkinsUtils.setProperty("admTest/appian-version-client/metrics.properties", "pipelineUsage", "true")
		  jenkinsUtils.setProperty("admTest/appian-import-client/metrics.properties", "pipelineUsage", "true")
          
        }
      }
    }
    
    
  }
}



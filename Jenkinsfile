pipeline {
	tools {
	  maven "MAVEN3"
	  jdk "OracleJDK8"

	}
    agent any

    stages {

      stage ("Fetch Code") {
        steps {
          git branch: "master", url: "https://github.com/PrasadVdm/CICD_Trivy.git"
        }
      }

      stage ("Unit test") {
        steps {
        	sh "mvn test"
        }
      }
    }
}

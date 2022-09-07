pipeline {
    agent any
    tools{
        maven "MAVEN3"
        jdk "OracleJDK8"
    }

    
    environment {
        SNAP_REPO = 'atostest-snap'
		NEXUS_USER = 'admin'
		NEXUS_PASS = 'admin123'
		RELEASE_REPO = 'atostest-release'
		CENTRAL_REPO = 'vpro-maven-central'
		NEXUSIP = '10.182.0.11'
		NEXUSPORT = '8081'
		NEXUS_GRP_REPO = 'atostest-group'
        NEXUS_LOGIN = 'nexusloginid-1'
    }


    stages {
       stage ('build'){

        steps {
              sh 'mvn -s settings.xml -DskipTests install'
           }
            
           } 
    }
}



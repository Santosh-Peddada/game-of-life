node('MAVEN') {

    stage('SCM'){
        //taking code from git
        git 'https://github.com/Santosh-Peddada/game-of-life.git'
    }

    stage('Build the package'){
        //code build
        sh 'mvn clean package'
    }

    stage('Archival'){
   // This step should not normally be used in your script. Consult the inline help for details.
    archive 'gameoflife-web/target/*.war'
    }

   }
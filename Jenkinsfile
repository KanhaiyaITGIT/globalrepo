pipeline {
    agent any
    environment {
        PATH = "/opt/maven/bin:$PATH"
    }

   stages {
        stage("git clone") {
             get url: "https://github.com/KanhaiyaITGIT/globalrepo.git", branch: "main"
        }

        stage("maven"" {
            steps {
             sh "mvn clean package"
            }
        }
   }
}

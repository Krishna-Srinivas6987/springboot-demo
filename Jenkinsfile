pipeline{
    agent any
    tools { maven "Maven" }
    stages{
     stage ('Build'){
            steps{
                sh "mvn clean install"
            }
        }
    /*stage('Sonar') 
       {environment {
           scannerHome=tool 'sonarScanner'
       }
            steps {
                withSonarQubeEnv('SonarQube') {
                sh "mvn sonar:sonar"
                }
            }
        }
        stage("Quality Gate") {
            steps {
              timeout(time: 1, unit: 'HOURS') {
                waitForQualityGate abortPipeline: true
              }
         }
        }
        stage ('Nexus'){
            steps{
                withCredentials([usernamePassword(credentialsId: 'Nexus_Credentials', passwordVariable: 'password', usernameVariable: 'username')]) {
                    sh label: '', script: 'curl -u $username:$password --upload-file target/springboot-0.0.1-SNAPSHOT.war http://18.224.155.110:8081/nexus/content/repositories/devopstraining/hexagon6/springboot-0.0.1-SNAPSHOT.war'
                }
       
        }
        }*/
        //stage('Deploy to Development'){
          //  steps{
            // deploy adapters: [tomcat8(credentialsId: 'tomcat', path: '', url: 'http://18.224.251.223:8000/')], contextPath: null, onFailure: false, war: '**/*.war'
            //}
        //}
        /*stage('Deploy to Ansible Master'){
            steps{
                sh 'scp -i /var/lib/jenkins/.ssh/id_rsa -r /var/lib/jenkins/workspace/springboot-app-demo/target/springboot-0.0.1-SNAPSHOT.war ansadmin@172.31.31.91:/projects'
                
            }
        }
        stage('Deploy to Test Server'){
             steps{
                 sh 'ssh -t -t -i /var/lib/jenkins/.ssh/id_rsa ansadmin@172.31.31.91 "ansible-playbook /opt/playbooks/playfile.yml"'
             }
        }
        stage('Deploy to Performance Server'){
             steps{
                 sh 'ssh -t -t -i /var/lib/jenkins/.ssh/id_rsa ansadmin@172.31.31.91 "ansible-playbook /opt/playbooks/performance.yml"'
             }
        }
        stage('Deploy to Production Server'){
             steps{
                 sh 'ssh -t -t -i /var/lib/jenkins/.ssh/id_rsa ansadmin@172.31.31.91 "ansible-playbook /opt/playbooks/production.yml"'
             }
        }*/
    }
}

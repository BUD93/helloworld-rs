pipeline {
    agent any
    stages 
    {
        stage('Build') 
        {
            steps 
            {
                echo 'hi'
                //bat 'mvn -B -DskipTests clean package'
                bat 'mvn compile'
            }
        }
        /*stage('Test') {
            steps {
                bat 'mvn test'
            }
            post {
                always {
                    junit 'target/surefire-reports/*.xml'
                }
            }
        }*/
        stage('Deliver') 
        { 
            steps 
            { 
                echo 'hi'
                //bat 'java -jar "C:/Program Files (x86)/Jenkins/jboss-cli-client.jar" -c --controller=remote+http://40.76.18.84:9990 --user=newad --password=abcd@1234 --command="deploy --force ./target/jboss-helloworld-rs-7.0.0.GA.war"'
            }
            
        }
    }
}

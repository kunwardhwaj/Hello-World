

pipeline {
    agent any
    stages {
        stage('Example') {
            steps {
                echo 'Hello World'
                

                script {
              
                    def props = readFile(file: 'inputfile.txt')
                    for (int i = 0; i < props.size(); ++i) {
                        echo "Testing the ${props[i]} file"
                    }
                }
            }
        }
    }
}

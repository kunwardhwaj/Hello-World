

pipeline {
    agent any
    stages {
        stage('Example') {
            steps {
                echo 'Hello World'
                def props = readProperties  file: '${WORKSPACE}/inputfile.txt'

                script {
                 
                    for (int i = 0; i < props.size(); ++i) {
                        echo "Testing the ${props[i]} file"
                    }
                }
            }
        }
    }
}

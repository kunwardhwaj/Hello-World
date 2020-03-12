

pipeline {
    agent any
    stages {
        stage('Example') {
            steps {
                echo 'Hello World'
                

                script {
              
                    def props = readFile(file: 'inputfile.txt')
                    repo = splitStringWithComma(props)

                    for (int i = 0; i < repo.size(); ++i) {
                        echo "Testing the ${repo[i]} file"
                    }
                }
            }
        }
    }
}

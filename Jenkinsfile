@Library("shared") _

pipeline{
    agent any
    
    stages{
        
        stage("hello"){
            steps{
                script{
                    hello()
                }
            }
        }
        
        stage("code"){
            steps{
                script{
                    clone("https://github.com/aakarshmiglani/django-notes-app.git","main")
                }
            }
        }
        
        stage("test"){
            steps{
                script{
                    test()
                }
            }
        }
    }
}

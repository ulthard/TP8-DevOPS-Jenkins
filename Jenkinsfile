pipeline{
    agent any
    environment {
        USER_NAME = "JOE"
        USER_COLOR = "RED"    
    }
    stages{
        stage("Lister les variables") {
            environment {
                USER_SPORT = "SOCCER"
                USER_COLOR = "BLUE"  
            }
            steps{
                echo "L'utilisateur est : ${env.USER_NAME}."
                echo "La couleur est : ${env.USER_COLOR}"
                echo "Le sport est : ${env.USER_SPORT}"
            }
        }
        stage("Utilisation des variables") {
            steps{
                echo "L'utilisateur est : ${env.USER_NAME}."
                echo "La couleur est : ${env.USER_COLOR}"
            }   
        }
    }
}

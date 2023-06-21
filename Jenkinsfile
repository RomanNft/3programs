pipeline {
    agent any

    stages {
        stage("Install Software") {
            steps {
                // Встановлення Mozilla Firefox
                sh 'sudo apt-get update'
                sh 'sudo apt-get install -y firefox'

                // Встановлення VLC
                sh 'sudo apt-get install -y vlc'

                // Встановлення Rhythmbox
                sh 'sudo apt-get install -y rhythmbox'
            }
        }

        stage("Verification") {
            steps {
                // Перевірка встановлених програм
                sh 'firefox --version'
                sh 'vlc --version'
                sh 'rhythmbox --version'
            }
        }
    }
}

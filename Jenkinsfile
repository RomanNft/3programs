pipeline {
    agent any

    stages {
        stage("Install Software") {
            steps {
                // Встановлення Mozilla Firefox
                sh 'sudo install -y firefox'

                // Встановлення VLC
                sh 'sudo install -y vlc'

                // Встановлення Rhythmbox
                sh 'sudo install -y rhythmbox'
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

pipeline {
    agent any

    stages {
        stage("Install Software") {
            steps {
                // Встановлення Mozilla Firefox
                sh 'sudo -n apt-get update'
                sh 'sudo -n apt-get install -y firefox'

                // Встановлення VLC
                sh 'sudo -n apt-get install -y vlc'

                // Встановлення Rhythmbox
                sh 'sudo -n apt-get install -y rhythmbox'
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

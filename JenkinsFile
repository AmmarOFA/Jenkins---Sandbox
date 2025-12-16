pipeline {
    agent any

    options {
        office365ConnectorWebhooks([[
            name: 'Office 365',
            url: "https://prod-08.canadacentral.logic.azure.com:443/workflows/757bda822f2240f789945eafdf43f7f0/triggers/manual/paths/invoke?api-version=2016-06-01&sp=%2Ftriggers%2Fmanual%2Frun&sv=1.0&sig=-IsBuvtNvdb_OGxx0Pg8XjM77vUTWrOaGujbeYt0Pi8",
            startNotification: true,
            notifySuccess: true,
            notifyAborted: true,
            notifyNotBuilt: true,
            notifyUnstable: true,
            notifyFailure: true,
            notifyBackToNormal: true,
            notifyRepeatedFailure: true,
            timeout: 30000,
            adaptiveCards: true,
            mentionCommitters: true,
            mentionDevelopers: true
        ]])
    }
    stages {
        stage('Example Build') {
            steps {
                sh ("-ls")
            }
        }


    }
}

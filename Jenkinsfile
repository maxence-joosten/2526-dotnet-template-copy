}node {
    stage('Checkout') {
        checkout scm
    }

    stage('Build') {
        sh 'docker run --rm -v /var/lib/docker/volumes/jenkins-data/_data/workspace/${JOB_NAME}:/workspace -w /workspace mcr.microsoft.com/dotnet/sdk:9.0 dotnet build Rise.sln'
    }
}

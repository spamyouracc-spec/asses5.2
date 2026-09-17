pipeline{
agentany
stages{
stage('Checkout') {
steps{
gitbranch: 'main', url: 'https://github.com/<student-username>/<repo-name>.git'
}
}
stage('GenerateReport') {
steps{
bat 'pythonapp.py'
}
}
stage('ArchiveReport'){
steps{
archiveArtifactsartifacts: 'report.txt',fingerprint:true
}
}
}
}

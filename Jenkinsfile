pipeline
{
agent any

    stages
{
environment
    {
        def mvnhome = tool name: 'Maven', type: 'maven'
    }
    stage('clone')
    {
    steps {
        git 'https://github.com/Bhavyasreethakur/MavenProject.git'
        }
    }
    stage('package')
    {
    steps {
        
        sh "${mvnhome}/bin/mvn package"
        }
    }
}
}

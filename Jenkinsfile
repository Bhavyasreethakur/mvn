pipeline
{
agent any
environment
    {
        def mvnhome = tool name: 'maven', type: 'maven'
    }
    stages
{

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

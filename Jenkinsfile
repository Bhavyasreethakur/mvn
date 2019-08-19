pipeline
{
agent any
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
        def mvnhome = tool name: 'Maven', type: 'maven'
        sh "${mvnhome}/bin/mvn package"
        }
    }
}
}

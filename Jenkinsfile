def workspace;
node
{
    stage('Checkout')
    {
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'isaradhi24', url: 'https://github.com/isaradhi24/helloworld.git']]])
        workspace =pwd()
    }
    stage('Static Code Analysis')
    {
        echo "Static Code Analysis"
    }
    stage('Build')
    {
        echo "Build the Code"
    }
    stage('Unit Testing')
    {
        echo "Unit Testing"
    }
    stage('Delivery')
    {
        echo "Deliver The Code"
    }
    stage('Complete')
    {
        echo "Pipeline Completed"
    }
}

def workspace
node
{ 
    stage('Checkout')
    {
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '2a865b44-656b-4b74-875d-2073bd245bf3', url: 'https://github.com/mysteriousmanish/github-repo']]])
        workspace = pwd()
    }
    stage('Static Code Analysis')
    {
        echo "Static Code Analysis"
    }
    stage('Build')
    { 
        echo "Build the Test code"
    }
    stage('Test')
    {
        echo "Test the Code"
    }
}

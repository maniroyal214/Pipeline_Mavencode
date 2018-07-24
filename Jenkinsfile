def workspace;
node
{
    stage('checkout')
    {
       checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '504', url: 'https://github.com/maniroyal214/Pipelinecode.git']]])
       workspace =pwd()
    }
    stage('static code analysis')
    {
        echo "static code analysis"
    }
    stage('withAnt')
    {
      withAnt(jdk: 'java-home') {
    // some block
}

    }
    stage('build')
    {
        echo "build the code"
    }
    stage('unit testing')
    {
        echo "unit testing"
    }
}

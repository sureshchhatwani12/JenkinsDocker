node('DOTNETCORE'){
    stage('SCM'){
        checkout([$class: 'GitSCM', branches: [[name:'*/main']], doGenerateSubmoduleConfiguration: false, extension: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/sureshchhatwani12/JenkinsDocker']]])        
    }
    stage('Build'){
        sh 'dotnet build /ConsoleApp1/ConsoleApp1'
    }
    stage('Test'){
        echo 'Execute unit tests'
    }
    stage('Package'){
        echo 'Zip it up'
    }
    stage('Deploy'){
        echo 'Push to deployment'
    }
}
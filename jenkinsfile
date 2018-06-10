def workspace;
node{
    stage("Build"){
        workspace = pwd()
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/mallammahk/maven.git']]])
 
        echo "build step"
    }
    stage("test"){
        echo "test step"
    }
    stage("deploy"){
        echo "deploy step"
    }
}

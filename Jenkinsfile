node('linux'){
  stage('test'){
  git 'https://github.com/luo05434/java-project.git'
  sh 'ant -f test.xml -v'
  junit 'reports/result.xml'
  }
  
  stage('build'){
  sh 'ant -f build.xml -v'
  }
  
  stage('deploy'){
    sh 'aws s3 cp /workspace/java-pipeline/dist/rectangle-${BUILD_NUMBER}.jar s3://luo05434-hw10-jenkins-output/rectangle-4.jar'
    
  }
}

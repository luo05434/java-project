node('linux'){
  stage('test'){
  git 'https://github.com/luo05434/java-project.git'
  sh 'ant -f test.xml -v'
  junit 'reports/result.xml'
  }
  
  stage('build'){
  sh 'ant -f build.xml -v'
  }
}

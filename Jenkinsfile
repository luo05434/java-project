node('linux'){
  stage('test'){
  git 'https://github.com/luo05434/java-project.git'
  sh 'ant -buildfile test.xml'
  junit 'reports/*.xml'
  }
}

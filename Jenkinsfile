pipeline{
agent any
tools{ gradle:'GRADLE'
jdk:'JDK'

}
stages{
stage('Checkout'){
steps{
git branch:'main',url:'https://github.com/smshubham2005/demogradle.git'
}
}
stage('Build'){
steps{
sh 'gradle build'
}
}
stage('Test'){
steps{
sh 'gradle test'}
}
stage('Run Application'){
steps{
sh 'gardle run'}

}
}
post{
success{
echo 'Build scuucess'}
failure{
echo 'failure'
}}
}


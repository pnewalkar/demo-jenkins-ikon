node{
   stage('SCM Checkout'){
     git 'https://github.com/pnewalkar/demo-jenkins-ikon'
   }
   stage('Compile-Package'){
      def mvnHome =  tool name: 'maven_3_5_0', type: 'maven'   
      sh "${mvnHome}/bin/mvn package"
   }
      stage('Deploy'){
      def mvnHome =  tool name: 'maven_3_5_0', type: 'maven'   
      sh "${mvnHome}/bin/mvn deploy"
   }
}

node{
   stage('SCM Checkout'){
      git 'https://github.com/jinkahari/web-app'
   }
   stage('Compile-Package'){
      def mvnHome = tool name: 'maven', type: 'maven'
      sh "${mvnHome}/bin/mvn clean package"
   }
   
}

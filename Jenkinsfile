node{
   stage('SCM Checkout'){
      git 'https://github.com/jinkahari/web-app'
      tool name: 'maven', type: 'maven'
   }
   stage('Compile-Package'){
      def mavenHome= tool name: 'maven', type: 'maven'
      sh "${mavenHome}/bin"
   }
   
}

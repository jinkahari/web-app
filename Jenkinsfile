node{
   stage('SCM Checkout'){
      git 'https://github.com/jinkahari/web-app'    
   }
   stage('Compile-Package'){
      sh 'mvn clean package'
   }
   
}

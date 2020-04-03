currentBuild.displayName = "online-shopping-#"+currentBuild.number
node{
   options {
       buildDiscarder logRotator(daysToKeepStr: '5', numToKeepStr: '7')
   }
   Stages { 
    stage('SCM Checkout'){
      git 'https://github.com/jinkahari/web-app'
    }
    stage('Compile-Package'){
      def mvnHome = tool name: 'maven', type: 'maven'
      sh "${mvnHome}/bin/mvn clean package"
    }
   //stage('Email Notification'){
     // mail bcc: '', body: '''Hi Welcome to Jenkins email alerts
      //Thanks,
      //Hari''', cc: '', from: '', replyTo: '', subject: 'Jenkins job', to: 'jinkahariforu@gmail.com'
   //}
   } 
}

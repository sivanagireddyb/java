node {
   // Mark the code checkout 'stage'....
   stage 'Checkout'
  git url: "https://github.com/sivanagireddyb/java.git", branch: 'master'
   sh "git clean -f && git reset --hard origin/master"
   // Checkout code from repository
   
  

   // Get the maven tool.
   // ** NOTE: This 'M3' maven tool must be configured
  
   def mvnHome = tool 'maven'

   // Mark the code build 'stage'....
   stage 'Build'
   // Run the maven build
   sh "${mvnHome}/bin/mvn clean install"
}

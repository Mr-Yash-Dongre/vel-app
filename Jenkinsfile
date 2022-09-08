pipeline{
       agent{
           node {
               label "built-in"
               customWorkspace "/mnt/projects"
}
}
      stages{
          stage('send this file to slave-1'){
              steps{
                  sh "chmod -R 777 index.html"   
                  sh "scp -r 23mayohio.pem index.html ec2-user@172.31.38.178:/mnt"
}
}
}
}

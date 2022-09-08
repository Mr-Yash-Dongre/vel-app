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
                  sh "chmod -R 777 23mayohio.pem"   
                  sh "scp -r -i '23mayohio.pem' /mnt/projects/index.html ec2-user@172.31.38.178:/slave-1"
}
}
}
}

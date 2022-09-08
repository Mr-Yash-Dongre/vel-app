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
                  sh "scp -v -r -i /mnt/projects/23mayohio.pem /mnt/projects/index.html ec2-user@13.58.113.197:/mnt"
}
}
}
}

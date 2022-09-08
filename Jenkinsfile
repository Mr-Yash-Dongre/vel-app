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
                  sh "chmod 400 index.html"   
                  sh "scp -r index.html ec2-user@172.31.38.178:/mnt/slave-1"
}
}
}
}

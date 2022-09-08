pipeline{
       agent{
           node {
               label "built-in"
               customWorkspace "/mnt/projects"
}
}
      stages{
          stage('install httpd'){
              steps{
                  sh "yum install httpd -y"
                  sh "cp -r index.html /var/www/html/"
                  sh "chmod -R 777 /var/www/html/index.html"
                  sh "service httpd start"
}
}
}
}

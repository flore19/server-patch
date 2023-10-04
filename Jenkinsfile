pipeline {
  agent { 
    label "ansible-server"
  }
  stages { 
    stages ("deploy patch playbook"){
      steps{
        dir("/home/ec2-user/ansible-dev"){
          sh "ansible-playbook patch.yml"
        }
      }
    }
  }
}
    

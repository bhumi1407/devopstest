node {

  //agent any

  

    cleanWs()

    stage('Deploy to Kubernetes') {

        git branch: 'dev', credentialsId: 'token-git', url: 'https://github.com/bhumi1407/devopstest.git'
        env.image_name = readFile 'image_deploye.txt'
        sh '''
          #!/bin/bash
          cd ansible
          chmod 400 devopskey.pem
          ansible-playbook -i hosts site.yaml -e "@group_vars/${BRANCH_NAME}.yaml" -e "imagename=${image_name}" -e "target=dev"

        '''
      

    }

    
  

}

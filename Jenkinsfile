pipeline {

  agent any

  options {

    buildDiscarder logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '5', daysToKeepStr: '', numToKeepStr: '5')

  }

  stages {

    stage('check ansible') {

      steps {
        
        sh '''

          nginximagename = $(cat nginx_image_name)
          cd ansible
          ls -lrt
          pwd
          chmod 400 devopskey.pem
          ls -lrt
          #grvars = ${BRANCH_NAME}
          ansible-playbook -i hosts site.yaml -e "@group_vars/${BRANCH_NAME}.yaml" -e "imagename=${nginximagename}" -e "target=dev"

        '''

      }

    }

    
  }

}

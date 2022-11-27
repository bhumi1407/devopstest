node {

  //agent any

  

  

    stage('check ansible') {

      
        def time = "out"
        sh '''

          #nginximagename = $(cat nginx_image_name)
          cd ansible
          ls -lrt
          pwd
          chmod 400 devopskey.pem
          ls -lrt
          echo $time
          #echo ${nginximagename}
          #ansible-playbook -i hosts site.yaml -e "@group_vars/${BRANCH_NAME}.yaml" -e "imagename=$(echo $nginximagename)" -e "target=dev"

        '''

      

    }

    
  

}

node {

  //agent any

  

  

    stage('check ansible') {

      
        def time = "out"
        println(time)
        sh '''

          #nginximagename = $(cat nginx_image_name)
          cd ansible
          echo \${time}
          #echo ${nginximagename}
          #ansible-playbook -i hosts site.yaml -e "@group_vars/${BRANCH_NAME}.yaml" -e "imagename=$(echo $nginximagename)" -e "target=dev"

        '''
      

    }

    
  

}

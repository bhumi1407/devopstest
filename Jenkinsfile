node {

  //agent any

  

  

    stage('check ansible') {

      
        def time = "out"
      def testing = readFile '${WORKSPACE}/nginx_image_name.txt'
        println(testing)
        sh '''
          #!/bin/bash

          #declare nginximagename = nginx_image_name.txt
          cd ansible
          #echo "\${time}"
          #echo ${nginximagename}
          #ansible-playbook -i hosts site.yaml -e "@group_vars/${BRANCH_NAME}.yaml" -e "imagename=$(echo $nginximagename)" -e "target=dev"

        '''
      

    }

    
  

}

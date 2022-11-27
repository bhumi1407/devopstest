node {

  //agent any

  

    cleanWs()

    stage('check ansible') {

        git branch: 'prod', credentialsId: 'token-git', url: 'https://github.com/bhumi1407/devopstest.git'
        def time = "out"
        def testing = readFile 'image_deploye.txt'
        sh 'ls & pwd'
        println(testing)
        sh '''
          #!/bin/bash
          ls
          #declare nginximagename = nginx_image_name.txt
          cd ansible
          #echo "\${time}"
          #echo ${nginximagename}
          #ansible-playbook -i hosts site.yaml -e "@group_vars/${BRANCH_NAME}.yaml" -e "imagename=$(echo $nginximagename)" -e "target=dev"

        '''
      

    }

    
  

}

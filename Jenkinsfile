node {

  //agent any

  

    cleanWs()

    stage('check ansible') {

        git branch: 'prod', credentialsId: 'token-git', url: 'https://github.com/bhumi1407/devopstest.git'
        def time = "out"
        env.testing = readFile 'image_deploye.txt'
        //println(testing)
        sh '''
          #!/bin/bash
          ls
          cd ansible
          printenv
          #echo "${env.testing}"
          #echo ${nginximagename}
          #ansible-playbook -i hosts site.yaml -e "@group_vars/${BRANCH_NAME}.yaml" -e "imagename=$(echo $nginximagename)" -e "target=dev"

        '''
      

    }

    
  

}

node {
    stage 'Building image'
    git 'https://github.com/caxqueiroz/docker-springboot-jenkins-example' // checks out Dockerfile
    def myEnv = docker.build 'cqueiroz:snapshot'
    myEnv.inside {
        sh 'mvn clean package'
    }
}
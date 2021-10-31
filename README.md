# dev-in-docker-cpp
C++ geliştirme işini docker içinde yapalım

Komutlar:

```
docker rm -f jenkmaster; `
docker build -t dev/jenkins-master -f Dockerfile-jenkins-master . ; `
docker run -d `
--name jenkmaster `
-p 8083:8083 `
-v ${PWD}\jcasc_plugin_confs\casc.yaml:/var/jenkins_home/casc.yaml `
dev/jenkins-master
```


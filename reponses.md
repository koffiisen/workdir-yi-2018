# TP RealWorld


# 6.3.1
  * SHA1 7a2e472d9d9e77ad7de8f4ace9e09d7597ee60f7

# 6.3.2
  * https://github.com/mkenney/docker-npm/blob/master/node-8-debian/Dockerfile
  * volume src

  * docker image pull mkenney/npm:node-8-debian
  * Image ID : 9af19a7f4e2c

# 6.3.3
  * docker container run --rm -i -v $(pwd):/src mkenney/npm:node-8-debian npm install

# 6.3.4
  * docker container run --rm -i -v $(pwd):/src -p 8000:8080 mkenney/npm:node-8-debian npm run dev

# 6.4.1
  * SHA1 eef3d052fe83dc688c0eb3dab97876d714a2d14d

# 6.4.2
  * docker image pull gradle:4.7.0-jdk8-alpine
  * Image ID f438b7d58d0a
  * Volume déclaré /home/gradle/.gradle

# 6.4.3
  * docker volume create gradle-home
  * docker volume ls
  * Liste des Volumes : 
    *  DRIVER              VOLUME NAME
    *  local               1d4184c08e8fa5c620dbcd84e254dcf2979fda337b45c0e7faaf71e44ebbc845
    *  local               gradle-home
 

# 6.4.4
  * docker container run --rm -ti -v $(pwd):/src -v gradle-home:/home/gradle/.gradle -w /src gradle:4.7.0-jdk8-alpine gradle build

# 6.4.5
  * docker container run --rm -ti -v $(pwd):/src -v gradle-home:/home/gradle/.gradle -p 8001:8080 -w /src gradle:4.7.0-jdk8-alpine gradle bootRun
  ``` Réponse de l'url
	{"articles":[],"articlesCount":0}
  ```

# 6.5.1 
   
``` Local articles
{"articles":[{"id":"b8624864-62f9-4ed3-8295-5cfa00495c92","slug":"nathan-tg","title":"Nathan Tg","description":"Just Tg ( Natahn)","body":"Now Tg nathan","favorited":false,"favoritesCount":0,"createdAt":"2018-05-16T13:49:19.156Z","updatedAt":"2018-05-16T13:49:19.156Z","tagList":[],"author":{"username":"tg","bio":"","image":"https://static.productionready.io/images/smiley-cyrus.jpg","following":false}}],"articlesCount":1}

```

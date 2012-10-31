REPO_ID=vivosys-repo
REPO_URL=https://tools.vivosys.com/artifactory/ext-release-local
mvn -DrepositoryId=$REPO_ID -Durl=$REPO_URL \
  -Dfile=target/akka-kryo-serialization.jar \
  -DgroupId=com.romix.akka -DartifactId=akka-kryo-serialization -Dversion=0.1.0.vivo_1 \
  deploy:deploy-file

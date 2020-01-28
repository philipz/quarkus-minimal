# Quarkus Framework Docker image minimal by Native Image & ldd
1. Check project is workable. `./mvnw compile quarkus:dev`
2. Genernate native image file. `./mvnw package -Pnative -Dquarkus.native.container-runtime=docker`
3. Create minimal Docker image. `docker build -f src/main/docker/Dockerfile -t YOURNAME/IMAGE:minimal .

### Note: Docker must be install



###  run the compose file to start sql database and redis-cache service

```
docker-compose up
```

### build image - 

```
./mvnw spring-boot:build-image
```


### run server
```
./mvnw spring-boot:run -Dspring-boot.run.profiles=mysql
```

## Updates for integrating redis-chache- 

### Added Dependencies for redis- 

https://github.com/Kushagra-234/Collpollass/blob/a2fc96ad07de3618eb00399971304934de722bca/pom.xml#L63-L77
### Added redis Service in compose-file

https://github.com/Kushagra-234/Collpollass/blob/main/docker-compose.yml#L26-L34
### Updated cache config file

https://github.com/s-pratyush/spring-project/blob/90fffcab0e2c4d7f85db6332cdbfa0b010cdd528/src/main/java/org/springframework/samples/petclinic/system/CacheConfiguration.java#L1-L72


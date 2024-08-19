Execute following commands in the CMD:

#will execute application.properties
./gradlew bootRun

#will execute application-ldev.properties
./gradlew bootRun --args='--spring.profiles.active=-ldev'


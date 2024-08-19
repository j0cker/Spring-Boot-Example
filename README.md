Execute following commands in the CMD:

#will execute application.properties

./gradlew bootRun

#will execute application-ldev.properties

./gradlew bootRun --args='--spring.profiles.active=ldev'

Execute through IntelliJ

Run/Debug Configurations -> edit configurations -> plus button -> gradle -> gradle spring boot

environment variables -> create new: 
    name -> spring.profiles.active
    value -> ldev


//FOR GRADLE

Execute following commands in the CMD:

#will execute application.properties

./gradlew bootRun

#will execute application-ldev.properties

./gradlew bootRun --args='--spring.profiles.active=ldev'

//FOR MAVEN

in the pom.xml you need to add inside properties the next versions depending on the compatibility with your maven, JDK and spring boot versions:

  &lt;properties>
  
    <java.version>21</java.version>
    
    <maven.compiler.source>21</maven.compiler.source>
    
    <maven.compiler.target>21</maven.compiler.target>
    
  &lt;/properties>

//general conf for spring boot in intelliJ

Execute through IntelliJ

Run/Debug Configurations -> edit configurations -> plus button -> gradle -> gradle spring boot

environment variables -> create new: 
    name -> spring.profiles.active
    value -> ldev

//for resource -> properties

  you can change the extensions of .properties to .yaml to have jerarquies 

//errors

noresourcefoundexception no static resource

  Descubrí que la aplicación estaba en un paquete y debería tener el mismo nivel que el main de Java. Mete los controladores al mismo nivel de carpeta/paquetes

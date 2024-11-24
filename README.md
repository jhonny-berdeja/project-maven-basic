Execute mvn archetype:generate -DgroupId=com.jberdeja -DartifactId=project-maven-basic -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false  
-El comando archetype:generate permite seleccionar una plantilla (archetype) y generar un proyecto basado en ella.  
-DgroupId: Define el identificador único del proyecto, generalmente el dominio de tu organización al revés (por ejemplo, com.ejemplo).  
-DartifactId: Es el nombre del proyecto o módulo (por ejemplo, mi-proyecto).  
-DarchetypeArtifactId: Especifica la plantilla del proyecto, en este caso, maven-archetype-quickstart, que crea un proyecto Java básico.  
-DinteractiveMode=false: Ejecuta el comando sin preguntas interactivas.  
Added to pom   
  <properties>  
      <maven.compiler.source>17</maven.compiler.source>  
      <maven.compiler.target>17</maven.compiler.target>  
  </properties>  

Added file .gitignore -> /target/  
Execute mvn exec:java -Dexec.mainClass="com.jberdeja.App" or java -cp target/classes com.jberdeja.App  
 In the folder of pom execute  
git init  
git add .  
git commit -m "first commit"  
git remote https://github.com/jhonny-berdeja/project-maven-basic.git  
the password is token access  
git push origin master  


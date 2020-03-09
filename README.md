# Sample repo to reproduce a bug in IntelliJ lombok plugin

## Reproduction:
- `mvn install` => it should works
- open MainClass in IntelliJ
- reformat the code
- `mvn install` throws
```
[ERROR] Failed to execute goal org.apache.maven.plugins:maven-compiler-plugin:3.1:compile (default-compile) on project lombokReproUtilityClass: Compilation failure: Compilation failure: 
[ERROR] /home/masterprice/dev/lombokReproUtilityClass/src/main/java/foo/MainClass.java:[3,1] cannot find symbol
[ERROR]   symbol:   static sayHello
[ERROR]   location: class foo.MyUtilityClass
[ERROR] /home/masterprice/dev/lombokReproUtilityClass/src/main/java/foo/MainClass.java:[8,5] cannot find symbol
[ERROR]   symbol:   method sayHello()
[ERROR]   location: class foo.MainClass
[ERROR] -> [Help 1]
```

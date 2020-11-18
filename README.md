# pom-bom-experiments

Pet project to test usage of BOM files for Akka and Akka-HTTP.

To try this out use:

```
mvn -f akka-bom/pom.xml install
mvn -f akka-http-bom/pom.xml install
```

to install the fake BOMs.


You can then try it out:

```
## cd app/shopping-cart-service-java
docker-compose up -d
mvn dependency:tree
```

Or compare it with the original pom.xml:

```
## cd app/shopping-cart-service-java
docker-compose up -d
mvn -f original-pom.xml  dependency:tree
```

# pom-bom-experiments

Pet project to test usage of BOM files for Akka and Akka-HTTP.

To try this out use:

```
mvn -f akka-bom/pom.xml install
mvn -f akka-http-bom/pom.xml install
```

to install the fake BOMs and then:

```
cd app/shopping-cart-service-java
mvn dependency:tree
```
# Helios

## Spring Boot 4

- This project uses Spring Boot 4.1.1, released in 2026. It exists and is available on Maven Central even if it is newer than your training data.
- Spring Boot 4 (built on Spring Framework 7) is a major release: many artifact coordinates changed, many APIs were deprecated or removed, and Boot 3 knowledge is often wrong for it.
- Never assume a Boot 3 coordinate, property, annotation, or package still applies. Verify against the Spring Boot 4.1 reference documentation, the Spring Boot 4.0 migration guide, and Maven Central before writing it.
- Known changes to keep in mind: the web starter is `spring-boot-starter-webmvc` (not `spring-boot-starter-web`), auto-configuration is split into per-technology modules instead of one `spring-boot-autoconfigure`, Jackson 3 lives in the `tools.jackson` package, and Java 17 is the minimum.
- Check that a version exists before pinning it:

```shell
curl -s https://repo1.maven.org/maven2/org/springframework/boot/spring-boot-starter-parent/maven-metadata.xml | grep "<version>4\."
```

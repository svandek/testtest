# Building with a buildpack

```
pack build acnafklmdemo.azurecr.io/petclinic \
           --builder paketobuildpacks/builder:base \
           --volume "$(pwd)/binding:/platform/bindings/application-insights" \
           --path ../target/petclinic.war
```
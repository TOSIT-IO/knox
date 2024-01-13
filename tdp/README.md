# Knox TDP

## Build

```
mvn clean install \
  -Prelease \
  -Ppackage \
  -Drat.numUnapprovedLicenses=1000 \
  -DskipTests \
  -Dmaven.javdoc.skip=true \
  -Dcheckstyle.skip=true \
  -Dfindbugs.skip=true \
  -Dspotbugs.skip=true \
  --batch-mode \
  -fae
```

## Test

```
mvn clean test \
  -Panalyze \
  --batch-mode \
  --fail-never
```

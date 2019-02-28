# CloudSync

CloudSyncc is a simple command line tool that synchronizes a local file system structure to your Google Drive (and back):


### Integration tests

Integration tests are written with [JUnit](http://junit.org/) and reside under `src/test/java`. The class names have
to start with `IT` in order to distinguish them from normal unit tests. To run the integration tests place a valid authentication
file under `src/test/resources/.jdrivesync` and execute them with (as they are not executed during a normal build):

```
mvn test -Pintegration-test
```

Please use a separate Google account for these integration tests as they are written to delete and to list all
files of the account.

### Continous Integration

[Travis CI](https://travis-ci.org) build: ![Build Status](https://travis-ci.org/siom79/jdrivesync.svg)

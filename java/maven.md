# Apache Maven

## Installation

The installation of Apache Maven is a simple process of extracting the archive and adding the `bin` folder with the `mvn` command to the `PATH`.

* Ensure `JAVA_HOME` environment variable is set and points to your JDK installation

* Download [Apache Maven archive](http://maven.apache.org/download.cgi) and extract as:

```
$ unzip apache-maven-3.6.0-bin.zip
or 
$ tar xzvf apache-maven-3.6.0-bin.tar.gz
```

Set the location of `apache-maven-3.6.0` extracted as `M2_HOME`. You can add it to `~/.zshrc` profile. Also, add the `bin` directory of this to `PATH`.

```
$ export M2_HOME=/Users/apoorvam/apache-maven-3.6.0
$ export PATH=$PATH:$M2_HOME/bin
```

To verify installation, you can run `mvn -version`: 

```
$ mvn -version
Apache Maven 3.6.0 (97c98ec64a1fdfee7767ce5ffb20918da4f719f3; 2018-10-24T14:41:47-04:00)
Maven home: /Users/apoorvam/apache-maven-3.6.0
Java version: 1.8.0_65, vendor: Oracle Corporation, runtime: /Library/Java/JavaVirtualMachines/jdk1.8.0_65.jdk/Contents/Home/jre
Default locale: en_US, platform encoding: UTF-8
OS name: "mac os x", version: "10.14.2", arch: "x86_64", family: "mac"
```



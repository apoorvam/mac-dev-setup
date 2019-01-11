# Java

## Installation

You can check if Java is already installed in your system by running:

```
$ java -version
java version "1.8.0_65"
Java(TM) SE Runtime Environment (build 1.8.0_65-b17)
Java HotSpot(TM) 64-Bit Server VM (build 25.65-b01, mixed mode)

```

If you don't see an output like above, you can install java on your system. 

### Using Homebrew

```
brew update
brew tap caskroom/versions
brew cask install java    # Install latest version of Java
brew cask install java8   # Install Java 8
```

### Set JAVA_HOME

You need to set `JAVA_HOME` environment variable, you can also add it to your `~/.zshrc` or similar profile. 

```
$ export JAVA_HOME=/Library/Java/JavaVirtualMachines/jdk1.8.0_65.jdk/Contents/Home
```


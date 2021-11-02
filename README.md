# Embulk

Embulk helps in transferring data between types of databases, storages, file formats, cloud services, and else.

## Installation

Requirements:  
Embulk v0.9 and v0.10 run on Java 8. (Java 9 is not supported officially)

### Embulk

```sh
curl --create-dirs -o ~/.embulk/bin/embulk -L "https://dl.embulk.org/embulk-latest.jar"
chmod +x ~/.embulk/bin/embulk
echo 'export PATH="$HOME/.embulk/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```

### Java 8

Check version

```sh
java --version
```

Update repositories and install OpenJDK version 8

```sh
sudo apt-get update
sudo apt-get install openjdk-8-jdk
```

If version is not set correctly (if multiple versions of Java is installed), change java version:

```sh
sudo update-alternatives --config java
```

![select_java]

Java installation docs:  
<https://www.digitalocean.com/community/tutorials/how-to-install-java-with-apt-on-ubuntu-18-04>
<https://docs.datastax.com/en/jdk-install/doc/jdk-install/installOpenJdkDeb.html>

## Examples

- [example-01]: CSV in GZip file to StdOut
- [example-02]: CSV to GZip file
- [example-03]: CSV to PostgreSQL
- [example-04]: PostgreSQL to MySQL

<!-- Links -->
[example-01]: ./example-01/
[example-02]: ./example-02/
[example-03]: ./example-03/
[example-04]: ./example-04/

<!-- Images -->
[select_java]: ./screenshots/screen-001.png

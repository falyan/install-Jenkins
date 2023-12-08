# install-Jenkins Ubuntu 20.04 LTS
How to install Your Own Jenkins

Jenkins installers are available for several Linux distributions like 

- Debian/Ubuntu

- Fedora

- Red Hat/Alma/Rocky

this tutorial will use ubuntu 20.04 LTS

# Prerequisites
## server VPS (Virtual Private Server)

- Minimum hardware requirements:

| RAM | Disk Space    | OS              |
| :-------- | :------- | :------------------------- |
| `256 MB` | `1 GB` | UBUNTU 20.04 LTS |


- Recommended hardware configuration for a small team:

| RAM | Disk Space    | OS              |
| :-------- | :------- | :------------------------- |
| `4 GB` | `50 GB` | UBUNTU 20.04 LTS |

## Software requirements:
 
- [java verison 11+](https://www.jenkins.io/doc/book/platform-information/support-policy-java/)</br>
- chrome (to acces your jenkins server)
- jenkins.war

### step 1 install java 11
```bash
  apt install openjdk-11-jdk-headless
```
![Alt text](image.png)

### step 2 download generic latest version jenkins (extension .war)
```bash
  mkdir jenkins
```
```bash
  cd jenkins
```
```bash
  wget https://get.jenkins.io/war-stable/2.426.1/jenkins.war
```
```bash
  ls
```
![Alt text](image-1.png)

### run file jenkins.war with customes port, add & for runninf in the backround 
```bash
  java -jar jenkins.war --httpPort=7070 &
```
![Alt text](image-2.png)






                                                                    # Distributed System
### Pre-requisites:

1. JDK-8

        sudo apt-get remove openjdk*
        sudo apt update
        sudo apt install openjdk-8-jdk openjdk-8-jre
        java -version // it should have version start with 1.8... etc 
    
3. Download [MPJ Express](https://sourceforge.net/projects/mpjexpress/files/releases/mpj-v0_44.tar.gz/download) & extract in Downloads         
 
4. Install Apache Netbeans (It will be Easier to work with Netbeans on Windows than Ubuntu)
            
         sudo apt update && sudo apt upgrade
         sudo snap install netbeans --classic
     Glassfish server version must be 4.1.1

### Assignment 1:

Terminal 1:

    javac *.java
    rmic AddServerImpl

Terminal 2:

    rmiregistry

Terminal 3:

    java AddServer

Terminal 4:

    java AddClient 127.0.0.1 5 8  // The Number of Arguments are Specified after localhost address.

### Assignment 2: (if You are getting error in this or next assignment then issue is with Java Version it works with Java 8 only as it is depreciated after Java 8 :)     
Terminal 1:

    idlj -fall ReverseModule.idl
    javac *.java ReverseModule/*.java
    orbd -ORBInitialPort 1056&
    java ReverseServer -ORBInitialPort 1056& 

Terminal 2:

    java ReverseClient -ORBInitialPort 1056 -ORBInitialHost localhost

### Assignment 3: (Specify Path Properly Don't Just Copy Paste the Command ;)

Terminal:

    export MPJ_HOME=/home/ubuntu/Downloads/mpj-v0_44
    export PATH=$MPJ_HOME/bin:$PATH
    javac -cp $MPJ_HOME/lib/mpj.jar ArrSum.java
    $MPJ_HOME/bin/mpjrun.sh -np 4 ArrSum

### Assignment 4:

Terminal 1:

    python client.py


Terminal 2:

    python server.py

### Assignment 5:

Terminal

    javac Tring.java
    java Tring

### Assignmnet 6:

Terminal

    javac Bully.java
    java Bully
    javac Ring.java
    java Ring
    
### Assignment 7:

   [Youtube tutotial](https://www.youtube.com/watch?v=ASd1S-_HLWw&list=PL1ysxTqY226jlhxh31xMYS72CqC5_vodG&index=2)
   [Youtube tutorial](https://www.youtube.com/watch?v=0z-HvSfr-M4)
    
    

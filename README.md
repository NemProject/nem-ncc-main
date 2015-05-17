# nem-ncc-main

This is parent repository for NEM Community Client.

In few easy steps (more posts will follow).

Preliminaries:

 * **JDK** (not jre) installed (http://www.oracle.com/technetwork/java/javase/downloads/index.html)
 * Maven installed (https://maven.apache.org/download.cgi)


Punch it, Chewie!

* Clone the repository and checkout master branch
    1. `> git clone --recursive git@github.com:NewEconomyMovement/nem-ncc-main.git`
    2. `> cd nem-ncc-main`
    3. `> git submodule foreach git checkout -B master origin/master`
* `> mvn`

```
    [INFO] Reactor Summary:
    [INFO]
    [INFO] NEM Core ........................................... SUCCESS [01:20 min]
    [INFO] NEM Deploy ......................................... SUCCESS [  2.997 s]
    [INFO] NEM Community Client - NCC ......................... SUCCESS [ 10.391 s]
    [INFO] NEM Monitor ........................................ SUCCESS [  2.680 s]
    [INFO] NEM Console ........................................ SUCCESS [  1.852 s]
    [INFO] NEM Community Client - ALL ......................... SUCCESS [  0.020 s]
    [INFO] NEM Community Client - including dependencies ...... SUCCESS [  0.018 s]
    [INFO] ------------------------------------------------------------------------
    [INFO] BUILD SUCCESS
```

There are two http-related tests in nem.core that might occasionally fail.

(you can try passing -DskipTests=true to maven, although we discourage that)

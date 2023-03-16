![Leshan](https://eclipse.org/leshan/img/multicolor-leshan.png)

[Eclipse Leshan™](https://eclipse.org/leshan) is an OMA Lightweight M2M server and client Java implementation.

[What is OMA LWM2M ?](https://omaspecworks.org/what-is-oma-specworks/iot/lightweight-m2m-lwm2m/)  
[LWM2M Specifications](https://github.com/eclipse/leshan/wiki/Lightweight-M2M-Specification).  

Leshan provides libraries which help people to develop their own Lightweight M2M server and client.  
The project also provides a client, a server and a bootstrap server demonstration as an example of the Leshan API and for testing purpose.

| LWM2M Version <br> Targeted | Leshan  <br> Version | Minimal <br> Java Version | Development <br> State |  Build Status	|  Standalone <br> Demos |
| - | - | - | - | - | - |
| [v1.0.x](https://github.com/eclipse/leshan/wiki/Lightweight-M2M-Specification#lightweight-m2m-v10x) | [v1.x](https://github.com/eclipse/leshan/tree/1.x) <br/> [Supported features](https://github.com/eclipse/leshan/wiki/LWM2M-Supported-features) | Java 7 | stable released | [jenkins-1.x](https://ci.eclipse.org/leshan/job/leshan-1.x/) | [server-demo](https://ci.eclipse.org/leshan/job/leshan-1.x/lastSuccessfulBuild/artifact/leshan-server-demo.jar)<br/> [client-demo](https://ci.eclipse.org/leshan/job/leshan-1.x/lastSuccessfulBuild/artifact/leshan-client-demo.jar) <br/> [bsserver-demo](https://ci.eclipse.org/leshan/job/leshan-1.x/lastSuccessfulBuild/artifact/leshan-bsserver-demo.jar) |
| [**v1.1.x**](https://github.com/eclipse/leshan/wiki/Lightweight-M2M-Specification#lightweight-m2m-v11x)| [**v2.x** (master)](https://github.com/eclipse/leshan/tree/master) <br/> [Supported features](https://github.com/eclipse/leshan/wiki/LWM2M-1.1-supported-features) | Java 8 | **in development**  |[jenkins-master](https://ci.eclipse.org/leshan/job/leshan/)     | [server-demo](https://ci.eclipse.org/leshan/job/leshan/lastSuccessfulBuild/artifact/leshan-server-demo.jar)<br/> [client-demo](https://ci.eclipse.org/leshan/job/leshan/lastSuccessfulBuild/artifact/leshan-client-demo.jar) <br/> [bsserver-demo](https://ci.eclipse.org/leshan/job/leshan/lastSuccessfulBuild/artifact/leshan-bsserver-demo.jar)  |


Release (stable and milestones) are available on [maven central](https://search.maven.org/search?q=org.eclipse.leshan).  
Nightly build (snapshot) are available on [eclipse repo](https://repo.eclipse.org/#view-repositories;leshan-snapshots~browsestorage). ([more details](https://github.com/eclipse/leshan/pull/885))

The Leshan Documentation  is available in our [wiki :blue_book:](https://github.com/eclipse/leshan/wiki).

Contact
-------

Join the project mailing list : [subscribe](https://dev.eclipse.org/mailman/listinfo/leshan-dev).  
Mail address: leshan-dev@eclipse.org.  
Access to [leshan-dev archives](https://dev.eclipse.org/mhonarc/lists/leshan-dev/).  

License
-------

This work is dual-licensed under the Eclipse Public License v2.0 and Eclipse Distribution License v1.0

`SPDX-License-Identifier: EPL-2.0 OR BSD-3-Clause`

Test Server Sandbox
------------

You can try live our servers demos instances:

* The **lwm2m server** at https://leshan.eclipseprojects.io/  
   _(coap://leshan.eclipseprojects.io:5683  and coaps://leshan.eclipseprojects.io:5684)_  
* The **bootstrap server** at https://leshan.eclipseprojects.io/bs/  
   _(coap://leshan.eclipseprojects.io:5783  and coaps://leshan.eclipseprojects.io:5784)_  

(Automatic deployment of master branch)

![Leshan](https://www.eclipse.org/leshan/img/capture_for_github-v2.png)

Test Leshan Demos locally
-----------------------
Get and run the last binary of our demo **server** :
```
wget https://ci.eclipse.org/leshan/job/leshan/lastSuccessfulBuild/artifact/leshan-server-demo.jar
java -jar ./leshan-server-demo.jar
```
Get and run the last binary of our demo **client** :
```
wget https://ci.eclipse.org/leshan/job/leshan/lastSuccessfulBuild/artifact/leshan-client-demo.jar
java -jar ./leshan-client-demo.jar
```
Get and run the last binary of our **bootstrap** demo server :
```
wget https://ci.eclipse.org/leshan/job/leshan/lastSuccessfulBuild/artifact/leshan-bsserver-demo.jar
java -jar ./leshan-bsserver-demo.jar
```
:information_source: : _All the demos have a `--help` option._

Compile Leshan & Run Demos
-------------
Get sources :
```bash
#using ssh
git clone git@github.com:eclipse/leshan.git
```
or
```
#using https
git clone https://github.com/eclipse/leshan.git

```

Compile it, by running in leshan root folder :

```
mvn clean install
```

Run demo **server**:
```
java -jar leshan-server-demo/target/leshan-server-demo-*-SNAPSHOT-jar-with-dependencies.jar 
```

Connect on Leshan demo UI: http://localhost:8080  
Leshan server Demo provides a very simple UI to get the list of connected clients and interact with clients resources.

Now you can register a LWM2M client by running our **client** demo:
```
java -jar leshan-client-demo/target/leshan-client-demo-*-SNAPSHOT-jar-with-dependencies.jar 
```
or trying the [Eclipse Wakaama](http://eclipse.org/wakaama) test client.

You can also try our **bootstrap** demo server:
```
java -jar leshan-bsserver-demo/target/leshan-bsserver-demo-*-SNAPSHOT-jar-with-dependencies.jar 
```

Let's start to code !
---------------------
Now you played a bit with our demo, you should start to code your own server or client using our [Getting-started](https://github.com/eclipse/leshan/wiki/Getting-started) guide.

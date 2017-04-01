# FOREWORDS #
You can choose whatever language to implement the web API. We advise you to use pure C, and we give you starter code for that.

Other technologies available are: Go, Java EE, PHP, NodeJS, Ruby, Python....

We can help you with Java and Python, so for other languages you are on your own.

# Coding a WEB API in C#

## DEPENDENCIES ##

* c build environment
* gosap
* cmake
* bison 
* flex

```bash
sudo apt-get install build-essential gsoap libgsoap-dev cmake bison flex
```

## COMPILATION ##

just launch
```
./create_project_files.sh 
```

that will create makefiles for you in ./build and launch a build. Once created, You can just call make in the build directoty to perform a full build.

## TEST ##

### REST ###

Binaries are generated in the ./build/rest directories.
Open 2 terminals, and launch

```
./build/rest/REST_SERVER 
~~ listening on 8888
Waiting for connections...
```

then the client

```
./build/rest/REST_CLIENT 
France
Italy
England
```

you can also use directly a web browser (we use iceweasel) to test the rest API.

```
iceweasel http://localhost:8888/countries/France
```


## Using ECLIPSE or CLION##

You are advised to use an IDE such as ECLIPSE CDT or CLION, as it make the development and debugging easier





# Simple setup with python Anaconda Jupyter

### Download the source
```
$ git clone git@github.com:gBobCodes/simple-r-docker.git
$ cd simple-r-docker
```

### Build Docker Images
```
$ docker-compose build
```

### Start Anaconda container
```
$ docker-compose up -d conda
$ docker-compose stop conda (to stop it)
```
Anaconda is at localhost:8888

The token needed to access the jupyter notebooks is displayed in the 
console window that started the conda container. Something similar to this
```
http://127.0.0.1:8888/?token=416df0941ac328cfebf8b84fb81386d1a3c3cf1a6bc43ab2
```

### Start the database administration tool, adminer
```
$ docker-compose up -d adminer
$ docker-compose stop adminer (to stop it)
```
Adminer is at localhost:8088 , See .env file for credentials.


### NOTE: The DB connectors have not yet been tested.

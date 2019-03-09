# IT_learning_nodejs
node.js bootstrap vue.js express

### docker-infra

- Docker base javascript node.js example project  

- jupyter

```
    docker build -f Dockerfile.jupyter --tag mrsono0/IT_learning_nodejs:jupyter .
    docker run --rm -it -p 8888:8888 -e JUPYTER_ENABLE_LAB=yes mrsono0/IT_learning_nodejs:jupyter
    docker push mrsono0/IT_learning_nodejs:jupyter
```

- docker compose cli command

```
    docker-compose -f ./docker-compose.yml up
    docker-compose -f ./docker-compose.yml run workspace
    docker-compose -f ./docker-compose.yml run workspace /bin/bash
    docker-compose -f ./docker-compose.yml stop workspace
    docker-compose -f ./docker-compose.yml restart workspace
    docker-compose -f ./docker-compose.yml logs
    docker-compose kill -s SIGINT
    docker cp ./app_flask flask:/workspace/app
```

```
docker commit it_learning_python_workspace
docker commit -a "Foo Bar <foo@bar.com>" -m "add hello.txt" hello-nginx hello:0.2
docker tag it_learning_python:jupyterlab mrsono0/it_learning_python:jupyterlab
```
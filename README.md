# IT_learning_nodejs
node.js bootstrap vue.js express

### docker-infra

- Docker base javascript node.js example project  

- IDE : vscode + 분석 라이브러리

```
    docker build -f Dockerfile.ide --tag mrsono0/IT_learning_nodejs:ide .
    docker run --rm -itd -p 33890:3389 -p 2222:22 mrsono0/IT_learning_nodejs:ide
    docker tag IT_learning_nodejs:ide mrsono0/IT_learning_nodejs:ide
    docker push mrsono0/IT_learning_nodejs:ide
```

- jupyter + 분석 라이브러리

```
    docker build -f Dockerfile.jupyterlab --tag mrsono0/IT_learning_nodejs:jupyterlab .
    docker run --rm -it -p 8888:8888 -p 2222:22 -e JUPYTER_ENABLE_LAB=yes mrsono0/IT_learning_nodejs:jupyterlab
    docker tag IT_learning_nodejs:jupyterlab mrsono0/IT_learning_nodejs:jupyterlab
    docker push mrsono0/IT_learning_nodejs:jupyterlab
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
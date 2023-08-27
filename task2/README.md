## Чтобы воспользоваться API, проделайте следующие шаги: ##

1. Загрузите, установите и запустите [Docker Desktop](https://www.docker.com/products/docker-desktop/)

2. Скопируйте репозиторий: 
    ```
    git clone --branch docker2 --single-branch https://github.com/kievsan/stocks_products
    ```
3. Перейдите в директорию с файлом ***Dockerfile***, затем выполните сборку:
    ```
    docker build --tag stocks_products .
    ```
4. Запустите контейнер:
    ```
    docker run -d -p 8000:8000 --name stocks_products stocks_products
    ```
Чтобы остановить контейнер, выполните:
    ```
    docker container stop stocks_products
    ```

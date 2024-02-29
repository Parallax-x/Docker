# Папка html - первое задание

    Необходимо создать образ из папки html: docker build . --tag=nginx
    Запустить контейнер: docker run -d -p 8001:80 --name=nginx nginx
    Проверить работоспособность: curl localhost:8001/ 

# Папка project - второе задание

    Необходимо создать образ из папки stocks_products: docker build . --tag=app_1
    Запустить контейнер: docker run -d -p 8000:8000 --name=my_app app_1
    В браузере ввести в адресную строку: http://localhost:8000/api/v1/
        
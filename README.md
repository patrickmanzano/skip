# skip challenge

This challenge was focusing on using an 'Event-Carried State Transfer'concept where the product gets inserted/updated/deleted and it dispatches and event, the other (product) api(s) will listen and act by receiving the event and doing something about it (updating its information, or making the produc avaliable/unavaliable for use)

## Project Structure

![Project Structure](https://github.com/codemonkeybr/skip/blob/master/files/structure.png)

# How to Run it
* In order do keycloack work properly on docker and localhost enviroment add `127.0.0.1	keycloak` to your /etc/hosts file (Unix plataform, or find the hosts file and add it to windows plataform

1. `docker-compose up` will initalize databases, rabbitmq and keycloak
2. The module skip-cart will make the Cart API run
3. The module skip-product will make the Product API run

* Both apis are visible on swagger on at `http://localhost:8082/swagger-ui.html` (Cart API) and `http://localhost:8082/swagger-ui.html` (Product API) use user `user`and pass `pass` on both to authenticate.

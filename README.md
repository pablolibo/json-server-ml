#How to use


## Solo correr:
```
git clone repo
docker-compose up
```

##Preguntas:

### a) Permitir la subida de un json al pegarle a la uri /json con un POST, indicando el id del json en el cuerpo

```
curl -X POST -H "Content-Type: application/json" -d @new_json.json http://localhost:3000/json
```

### b) Servir el json cuando se hace un GET a /json/ 

```
curl -X GET -H "Content-Type: application/json"  "http://localhost:3000/json/2"
```

### c) Permitir la modificación del json cuando se hace un PUT a /json/ 

```
curl -X PUT -H "Content-Type: application/json" -d @modify_json.json "http://localhost:3000/json/2"
```

### d) Permitir la eliminación del json cuando se hace un DELETE a /json/ 

```
curl -X DELETE http://localhost:3000/json/2
```

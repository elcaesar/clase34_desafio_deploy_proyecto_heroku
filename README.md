## Desafío: clase 34: Despliege del proyecto a la nube

#### Pasos a seguir antes de hacer de desplegar a la nube el proyecto

* En el archivo `package.json` asegurarse que en la parte de `scripts` no se utilice el módulo `nodemon`, en su lugar se puede definir por ejemplo:
```
"start" : "node app.js"
```

* Heroku asigna automáticamente un puerto que tenga disponible por lo que si se definió a nivel un número de puerto, se debe borrar y definir:
```
const port = process.env.PORT || 8080
```

* Asi como si se define como variable de entorno una conexión a base de datos se debe especificar en heroku como el siguiente ejemplo:

[![environments.jpg](https://i.postimg.cc/vTLy7R48/environments.jpg)](https://postimg.cc/K3zCFH7C)


* el sitio web desplegado en Heroku es: https://deploy-app-clase34-nodejs.herokuapp.com/

[![deploy.jpg](https://i.postimg.cc/9f6zJhQy/deploy.jpg)](https://postimg.cc/3yZKxzpw)



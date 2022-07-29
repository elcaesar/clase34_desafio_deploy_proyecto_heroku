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



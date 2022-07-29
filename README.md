## Desafío: clase 34: Despliege del proyecto a la nube

#### Pasos a seguir antes de hacer de desplegar a la nube el proyecto

* En el archivo `package.json` asegurarse que en la parte de `scripts` no se utilice el módulo `nodemon`, en su lugar se puede definir por ejemplo:
```
"start" : "node app.js"
```

* se define en el archivo de variables globales (por ejemplo `.env`)
    -- DB_CONN = la cadena de conexión a la base de datos
    -- HOST = `localhost`
luego usar esas variables para poner el servidor en escucha.

No se define el puerto ya que Heroku lo asigna automáticamente, se puede definir así:
```
const port = process.env.PORT || 8080
```




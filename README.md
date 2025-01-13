<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="120" alt="Nest Logo" /></a>
</p>

# Ejecutar en desarrollo
1.clonar el repositorio
2.Ejecutar
```
npm install
```
3. Tener NEST CLI instalado
```
npm i -g @nestjs/cli
```
4. Levantar la base de datos
```
docker-compose up -d
```
5. Clonar el archivo __.env.template__ y renombrar la copia a __.env__

6. LLenar las variables de entorno definidas en el ```.env```

7. Ejecutar la aplicación en dev:
```
npm  run start:dev
```

8. Reconstruir la base de datos con la semilla
```
http://localhost:3000/api/v2/seed
```

## Stack usado
* Mongo DB
* Nest

## Production Build
1. Crear el archivo ```.env.prod```
2. LLenar las variables de entorno de prod
3. Crear la nueva imagen

```docker-compose -f docker-compose.prod.yaml --env-file .env.prod up --build```

# Final Drilling

- Para usar el proyecto debe instalar las dependencias: `npm install`

- Debe tomar en cuenta la configuracion de la base de datos:

```
module.exports = {
  HOST: 'localhost',
  USER: 'node_user',
  PASSWORD: 'node_password',
  DB: 'db_jwtbootcamp',
  dialect: 'postgres',
  pool: {
    max: 5,
    min: 0,
    acquire: 30000,
    idle: 10000
  }
}
```

- Una vez instalandas las dependencias podrá correr el servidor: `npm run dev`. Las rutas son las siguientes (Tambien puede realizar todas las consultas mencionadas usando el archivo de postman: m8_final_drilling.postman_collection)
  http://localhost:3000/

  - User

    - Crear Usuario: POST http://localhost:3000/api/signup (publica)
    - Iniciar Sesion: POST http://localhost:3000/api/signin (publica)
    - Ver Usuario: GET http://localhost:3000/api/user/:id (privada)
    - Ver Usuarios: GET http://localhost:3000/api/user (privada)
    - Modifcar Usuario: PUT http://localhost:3000/api/user/:id (privada)
    - Borrar Usuario: DELETE http://localhost:3000/api/user/:id (privada)

  - Bootcamp
    - Crear Bootcamp: POST http://localhost:3000/api/bootcamp (privada)
    - Agregar Usuario a Bootcamp: POST http://localhost:3000/api/bootcamp/adduser (privada)
    - Ver Bootcamp: GET http://localhost:3000/api/bootcamp/:id (privada)
    - Ver Bootcamps: GET http://localhost:3000/api/bootcamp (publica)

- Tambien puede ver los resultados de las consultas en la carpeta consultas:
  - Base de Datos: Usuarios ![Base de Datos: Usuarios](consultas/m8_0_bd_usuarios.png)
  - Base de Datos: Bootcamps ![Base de Datos: Bootcamps](consultas/m8_1_bd_bootcamps.png)
  - Base de Datos: Usuario / Bootcamps ![Base de Datos: Usuario / Bootcamps](consultas/m8_2_bd_usuario_bootcamp.png)
  - Registrase ![Registrase](consultas/m8_3_registrarse.png)
  - Registrase - Error ![Registrase - Error](consultas/m8_4_registrarse_error.png)
  - Iniciar Sesion ![Iniciar Sesion](consultas/m8_5_iniciar_sesion.png)
  - Ver Usuarios ![Ver Usuarios](consultas/m8_6_usuarios.png)
  - Ver Usuario ![Ver Usuario](consultas/m8_7_usario.png)
  - Modificar Usuario ![Modificar Usuario](consultas/m8_8_modificar_usuario.png)
  - Eliminar Usuario ![Eliminar Usuario](consultas/m8_9_eliminar_usuario.png)
  - Ver Bootcamp ![Ver Bootcamp](consultas/m8_10_bootcamp.png)
  - Ver Bootcamps ![Ver Bootcamps](consultas/m8_11_bootcamps.png)
  - Agregar Usuario a Bootcamp ![Agregar Usuario a Bootcamp](consultas/m8_12_bootcamp_agregar_usuario.png)
  - Agregar Bootcamp ![Agregar Bootcamp](consultas/m8_13_agregar_bootcamp.png)

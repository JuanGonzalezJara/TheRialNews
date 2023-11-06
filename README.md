Desafio Unidad 6 Modulo 2 (1)

#  Mecanismos de autenticación y control de accesos en una aplicación web!

Desafio orientado a validar conocimientos de mecanismos de autenticacion y control de accesos en una aplicacion web. 

## Requerimientos

1. Set-up inicial del proyecto con sus relaciones y modelos.
2. Agregar roles a los usuarios con sus permisos.
3. Si un usuario olvida su contraseña, puede recibir un email para restablecerla.
4. Las noticias deben tener sus tests funcionales.
5. Hacer deploy a heroku.


## Subiendo proyecto a Heroku

- Deberas tener primero instalado Heroku en tu instancia de desarrollo, puedes realizarlo siguiendo el proceso desde la web de [heroku](https://id.heroku.com/login).
- Tambien deberas tener tu proyecto con Git inicializado o contar con la carpeta .git en tu proyecto

1: En la terminal, inicia sesión en Heroku:

```bash
heroku login
```

2: Crea una aplicación en Heroku:

```bash
heroku create
```

- Es importante copiar el nombre de la aplicación proporcionado por Heroku

3: Ahora conectaremos el proyecto con nuestra aplicación en Heroku:

```bash
heroku git:remote -a nombre-proyecto-dado_por_heroku
```

4: Realiza un push a Heroku:

```bash
git push heroku main
```

5: Debes ir a la página de tu aplicación en la web de [heroku](https://id.heroku.com/login) y dirigirte a la pestaña de la derecha que dice "More", Una vez que se despliegue el menú, selecciona la opción "Run console".

![Logo!](https://raw.githubusercontent.com/JuanGonzalezJara/TwitterClon/main/app/assets/images/heroku_menu_console.png?token=GHSAT0AAAAAACEFOVVZ3IZDU5RD6TGA7XBSZJHG6RA)


6: Una vez que se despliegue la consola, asegúrate de crear la base de datos si aún no está creada, migrar los cambios y generar los datos mediante el archivo seed.rb:

```bash
rails db:create
rails db:migrate
rails db:seed
```

Siguiendo estos pasos ya podras ver el funcionamiento de la aplicacion con los datos generados por el seed.


![Logo!](https://raw.githubusercontent.com/JuanGonzalezJara/Desafio_RoR_Unidad4_M3_3/main/assets/ROR_Logo.png)

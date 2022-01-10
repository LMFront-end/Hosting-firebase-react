## hospedar un proyecto react en firebase 

1. Creamos una aplicación de react
   --> npx create-react-app
   nota: tener actualizdo node y npm (en caso de utilizar npm)

2. Creamos un nuevo proyecto en firebase
   ---> https://firebase.google.com

3. En el panel de firebase (compilación), seleccionamos hosting

4. En nuestra terminal, ingresamos los siguientes comandos:

## para instalar Firebase CLI

--> Firebase CLI es una herramienta de línea de comandos

** npm install -g firebase-tools

Una vez instaladas las herramientas, debemos iniciar sesión con una cuenta Google, para esto, debemos escribir el siguiente comando: 

** firebase login

Después de acceder e iniciar sesión con nuestra cuenta google, debemos iniciar el proyecto con el siguiente comando:

** firebase init

Una vez ejecutado el comando, veremos una serie de preguntas como:

 --> Are you ready to proceed? (Y/n)
  ** Si indicamos si: (y)

---> Veremos que servicios deseamos incluir en el proyecto:
** seleccionamos la opción que necesitamos, si el caso es solo hospedaje, seleccionamos:

(*) Hosting: Configure files for firebase hosting and (optionally) set up Github Action deploys

Una vez finalizado este paso, encontraremos esta pregunta:

--> but for now we'll just set up a default project.

? please select an option

> use an existing project
> create a new project
> add firebase to an existing cloud platform project

--> Si ya tenemos un proyecto de firebase creado desde la plataforma, seleccionaremos la primera opción. De lo contrario, seleccionamos crear uno nuevo.

Por ultimo:

? what do you want to use your public directory?

--> como estamos trabajando con react, debemos especificar la carpeta (build)

LLevando a cabo todos estos pasos, veremos que se ha creado una carpeta build, donde estarán los recursos react optimizados.

---> por último debemos hacer el deploy

con el siguiente comando:
** firebase deploy

--> lo que sucederá es que firebase tomara el contenido de build, lo va a cargar y lo hospedará, podremos ver los enlaces de hospedaje en la terminal.

+ Deploy complete!

## Project console: link
## Hosting URL: link








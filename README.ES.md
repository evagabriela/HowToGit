Explicacion de como utilizar Git de la manera basica que mas se utiliza:

En este articulo, se esta asumiendo que tiene un buen entendimiento de cómo usar terminal OSX o Linux para mobilizarse entre directorios y mostrar los contenidos usando los comandos `cd` y `ls`.

Es diferente usar Github que usar git. "git" en minúscula es el nombre el sistema de control de versiones (VCS o "version control system.") "Github" es un servicio web donde millones de repositorios git son colectados, y hay herramientas gráficas para examinarlos y compartirlos.

Por ejemplo, imagine que estoy trabajando en un proyecto que esta dentro de un repositorio, y deseo añadir mi nombre en una lista de colaboradores de un archivo README. 
Como aria esto?

1. Cree una cuenta en  Github si esque no la tiene. Tiene que saber su nombre de usuario y su clave.

2. Navegue al directorio dentro de su computadora donde quiera mantener estos proyectos. Por ejemplo: Yo tengo un directorio `/Users/ari/Projects/` donde se colocan todos mis proyectos pequeños (Recuerde que NO necesita crear un nuevo directorio para este nuevo proyecto, porque el comando `git clone` lo hará).

3. Vaya al direccion de URL del repositorio en Github con el cual desea trabajar. Aqui tendra que hace un clon ("clone") del repositorio para que una copia de este proyecto se guarde en su computadora. 

Haga clic sobre el botón "HTTP" en la página del repositorio. Copie el URL del repositorio, que empieza con "https" y termine con ".git" y pegue esto al lado de la palabra  `git clone` en el terminal y presione enter.

Por ejemplo:  Si esque tuviera un repositorio llamado "Treasury", entonces lo que pondras en el terminar lucira algo asi: 

`$ git clone https://github.com/tensory/Treasury.git`

4. Vaya al nuevo directorio que se ha creado. En mi ejemplo sería `/Users/ari/Projects/Treasury/`.

5. Crea un branch.

	__La Voz de Experiencia:__ Típicamente los tutoriales sobre git no empiezan con el concepto del branch. Yo creo que se deberia aprender esto primero. Al entender esto, podemos evitar muchos problemas con errores que se puedan crear en el branch principal.

	Un branch es una versión del repositorio donde se puede hacer cambios sin cometerlos en el branch principal, que se llama "master". Si esque no le gustan los cambios que hizo al branch, entoces tiene la opcion de borrarlo todo y empezar otra vez (sin causar ningún problema por master).

Ojo:  Escoja un buen nombre para el nuevo branch que estas creando en el cual le ayude recordar lo que intenta hacer con él. Es mejor crear un nuevo branch cuando tiene una tarea específica para completar. Usa el comando `git checkout` para crear 

# proyecto
Mi primer proyecto con Git 

###1. ¿Qué es git?
Git es un software de control de versiones diseñado por Linus Torvalds, pensando en la eficiencia y la confiabilidad del mantenimiento de versiones de aplicaciones cuando éstas tienen un gran número de archivos de código fuente. Su propósito es llevar registro de los cambios en archivos de computadora y coordinar el trabajo que varias personas realizan sobre archivos compartidos.

Los sistemas de control de versiones son programas que tienen como objetivo controlar los cambios en el desarrollo de cualquier tipo de software, permitiendo conocer el estado actual de un proyecto, los cambios que se le han realizado a cualquiera de sus piezas, las personas que intervinieron en ellos, etc.

El control de versiones es una de las tareas fundamentales para la administración de un proyecto de desarrollo de software en general. Surge de la necesidad de mantener y llevar control del código que vamos programando, conservando sus distintos estados. Es absolutamente necesario para el trabajo en equipo, pero resulta útil incluso a desarrolladores independientes.
> https://es.wikipedia.org/wiki/Git
> 
> **https://desarrolloweb.com/articulos/introduccion-git-github.html**

###2. ¿Por qué queremos utilizar git?
Queremos utilizar git porque nos permite gestionar las distintas versiones, etapas, ramas y estados de un proyecto en un grupo de trabajo mediante un repositorio centralizado en la nube. 

###3. ¿Qué es el bash que instala git?
Git Bash es una aplicación para Microsoft Windows que básicamente emula la línea de comandos de Git a través de una shell.

###4. Describa los estados (working directory, staging area, repository)

**El área de trabajo**, en resumen, son los archivos que no están en el área de preparación.
No son manejados por Git. Están en su directorio local. También se pueden llamar archivos sin seguimiento. El área de trabajo es como su espacio de memoria virtual, es donde puede agregar contenido nuevo, puede modificar eliminar contenido, si el contenido que modifica o elimina está en su repositorio, no tiene que preocuparse por perder su trabajo.

**El área de preparación**, eso es lo que los archivos van a ser parte de su próxima confirmación. Así es como Git sabe qué va a cambiar entre la confirmación actual y la próxima. Vamos a profundizar en el área de preparación en la siguiente sección. Brevemente, el repositorio, esos son los archivos que Git realmente conoce.


**El repositorio** contiene todos tus commits. Y el commit es una instantánea de cómo se ve su área de trabajo y puesta en escena en el momento del commit. Está en su directorio .git. Y esos son todos los archivos en su repositorio, están almacenados de forma segura, puede continuar haciendo cambios mientras trabaja y siempre puede retirar una copia nueva si la necesita.
  
###5. Describa el flujo para crear un nuevo repositorio git.

### Como crear un repositorio desde cero

*1.* Creamos una carpeta y un archivo en los cuales vamos a trabajar

> ejemplo
> 
> index.html
> 
> app.js

*2.* Inicializamos nuestro proyecto

> cd ejemplo
> 
> git init

*3.* Agregamos todos los archivos al repositorio

> git add .

*4.* Hacemos un commit de los archivos

> git commit -m "Ejemplo de como se utiliza git"

*5.* Creamos un repositorio en nuestra cuenta de github

*6.* Seguimos los pasos que nos informan estos sitios para subir nuestro repositorio ya creado

###6. Describa el flujo para agregar un archivo simple al repositorio.

Para agregar un archivo simple al repositorio de trabajo debemos: 

          Ej: git status
          git add (nombre del archivo)  
          git status 
          git commit


###7. Describa el flujo para cambiar el archivo agregado y guardar los cambios en el repositorio.

Luego de cambiar el archivo que habíamos agregado, debemos poner **git status** veremos que el archivo ha sido modificado y si queremos
ver las diferencias que realizamos decimos **git diff (nombre del archivo)** pero ese cambio que hicimos no se ha  sido agregado aún al
entorno de trabajo, para hacerlo debemos decir **git add (nombre del archivo)** nuevamente **git status** vemos que se agregó.
Para guardar los cambios decimos **git commit** se abrirá el editor para que ingresemos un mensaje.

      Ej: git status
          git diff (nombre del archivo)  
          git add (nombre del archivo) 
          git status
          git commit
          
          

###8. ¿Cómo hago para ignorar un archivo o carpeta?
   Para ignorar un archivo o carpeta debemos crear un carpeta llamada **.gitignore** allí alojaremos todo lo que no queremos en nuestro proyecto.

###9. Explique qué es un branch. Dé un pequeño ejemplo de cómo haría uno.
Branch es un comando en el que averiguamos donde estamos ubicados, en que versión del proyecto, al principio estamos en la rama "master".
Luego podemos realizar nuevas versiones con el mismo comando más el nombre que queramos que se llame y así creamos otra rama. 
git branch solamente crea una nueva rama, pero no salta a dicha rama.

     Ej: git branch
         * master 
          git branch login 
          git branch
          login
          * master


###10. ¿Qué hago con `git add .`?
     Con git add agrego archivos al "staging area" entorno de trabajo. 
     Ej: git add (nombre del archivo)  
###11. ¿Cómo cambiamos de un branch a otro?
    Con git checkout podemos cambiar de un branch a otro. 
     Ej: git checkout (nombre de la versión)

###12. Investigue qué es Markdown y responda todas las preguntas anteriores en este lenguaje (con el nombre de archivo RESPUESTAS.md).
Súbalo al repositorio.

## Markdown

Markdown es un lenguaje de marcado ligero creado por John Gruber que trata de conseguir la máxima legibilidad y facilidad de publicación 
tanto en su forma de entrada como de salida, inspirándose en muchas convenciones existentes para marcar mensajes de correo electrónico 
usando texto plano. Se distribuye bajo licencia BSD y se distribuye como plugin (o al menos está disponible) en diferentes sistemas 
de gestión de contenidos (CMS). Markdown convierte el texto marcado en documentos XHTML utilizando html2text creado por Aaron Swartz.
Markdown fue implementado originariamente en Perl por Gruber, pero desde entonces ha sido traducido a multitud de lenguajes de programación, 
incluyendo PHP, Python, Ruby, Java y Common Lisp.

> https://es.wikipedia.org/wiki/Markdown

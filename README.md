# Introducción

Git se ha vuelto un software indispensable a la hora de construir aplicativos móviles o web, ya sea si lo estas desarrollando de manera individual o grupal, dado que permite administrar versiones de código con mucha facilidad. Git te permitirá descargar un software, realizar cambios y subir dichos cambios a un servidor remoto o guardarlos de manera local. Si eres desarrollador web o desarrollador de aplicaciones móviles,  Git te será útil para cualquier tipo de aplicación que vayas a desarrollar y cuanto antes empieces a aprenderlo mejor provecho le darás a esta gran herramienta. Git cuenta con cientos de comandos, sin embargo, te voy a compartir 10 de los comandos GIT que son indispensables conocer si te encuentras colaborando en un proyecto de aplicaciones móviles o web.

# ¿Qué es Git?

En pocas palabras, Git es un sistema de control de versiones. Git te permitirá realizar un seguimiento de los cambios que se realice en los archivos, ya que, tiene un registro de lo que se ha hecho y gracias a ello se puede volver a versiones específicas si en caso se requiera. Git también agiliza las colaboraciones, ayudando que los cambios realizados por varias personas se fusionen en una sola fuente. Si trabaja de manera individual o de manera grupal, Git será útil para usted en cualquier circunstancia.

Git se ejecuta de manera local y por tal razón al momento de crear o modificar archivos se generará un historial en su computadora. Si en caso necesita que otros desarrolladores contribuyan con el aplicativo o software que está desarrollando y poder trabajar en paralelo, deberá subir el proyecto a una plataforma o servidor de alojamiento de código (como Github o Bitbucket).

## Configura tu nombre de usuario y tu correo electrónico con GIT CONFIG

Si estas iniciando en un proyecto y te han solicitado que instales Git, antes de usarlo deberás configurarlo. El comando git config te permitirá especificar el nombre de usuario y el correo electrónico que se establecerán al momento de realizar tus commits.

## ¿Cómo saber mi nombre de usuario y mi correo electrónico en Git?

Hay 3 maneras de poder conocer nuestro correo electrónico y el nombre de usuario que se encuentran configurados en Git.
              
1. Por medio del comando git config.
2. El comando git config --list  te detallará todas las propiedades que Git ha configurado.
3. A través del archivo de configuración .gitconfig.

#### 1. Por medio del comando git config

Si escribimos el siguiente comando git config user.name retornará el nombre de usuario que se encuentra configurado por defecto.

`$ git config user.name`

![image](https://user-images.githubusercontent.com/89370556/164998269-6b6492c8-f492-42a5-bd7b-52ec22b23723.png)

De igual forma podemos ver el correo electrónico que se encuentra configurado por defecto con el comando git config user.email.

`$ git config user.email`

![image](https://user-images.githubusercontent.com/89370556/164998328-6b7814e4-294e-47ab-a7f4-a67ab1bbc3ca.png)

#### 2. El comando git config –-list

Este comando nos brindará una explicación más detallada.

`$ git config --list`

![image](https://user-images.githubusercontent.com/89370556/164998390-06e2dd8b-0858-4cd6-811c-e15517b53af7.png)

#### 1. A través del archivo de configuración .gitconfig

Por último, podemos ver el nombre de usuario y el correo electrónico que se encuentran configurado en Git por medio de un archivo de configuración. Para ello, tenemos que buscar el siguiente archivo en la ruta de nuestro disco.

![image](https://user-images.githubusercontent.com/89370556/164998440-ab1a3cda-63ac-4554-9323-7cc63afddffc.png)

![image](https://user-images.githubusercontent.com/89370556/164998449-d0acd080-59f8-4ce5-a45e-cf99f82725fa.png)

Recuerda que Git está diseñado y optimizado para poder colaborar entre equipos, por esta razón, debemos de dar un poco de información sobre nosotros.

## ¿Cómo configurar el nombre de usuario y el correo electrónico de confirmación para Git?

Para poder configurar el nombre de usuario y el correo electrónico en Git debemos ejecutar los siguientes comandos:

Nombre de usuario:

`$ git config --global user.name "Tu Nombre"`

Correo Electrónico:

`$ git config --global user.email. "tu@email.com"`

![image](https://user-images.githubusercontent.com/89370556/164998508-a8df72a8-8ff3-47bb-9788-e1a9a50b2dc9.png)

Recuerda configurar tu información personal en Git antes de empezar a desarrollar cualquier proyecto dado que tus cambios serán enviados a un servidor remoto y tu equipo tendrá la necesidad de saber quien está realizando cambios en la rama correspondiente del proyecto.

## Clona los proyectos con el comando GIT CLONE

El comando Git Clone te permitirá descargar el código fuente existente desde un servidor remoto. Git Clone opera con una ruta (por lo habitual una URL) hacia el repositorio de Git que se necesite clonar. Tras ejecutar el comando Git Clone se generará una copia de trabajo local del código fuente del repositorio que se encuentra alojado en el servidor remoto. El código se generará automáticamente. Luego de haberse clonado el proyecto en su ruta local, si usted cuenta con los permisos necesarios, será capaz de aplicar cambios sobre el proyecto existente. Veamos un ejemplo de cómo clonar un repositorio con el comando Git Clone.

- Ingresamos al Servidor Remoto, buscaré un repositorio creado desde mi cuenta.

![image](https://user-images.githubusercontent.com/89370556/164998784-3971bf73-30fe-446e-94ba-ac198bc87b33.png)

![image](https://user-images.githubusercontent.com/89370556/164998789-74fdf679-9761-4417-8669-126c1c931d25.png)

Una vez dentro del repositorio, desplegamos el botón verde que dice Code y seleccionaremos (en este caso) la columna que dice “HTTPS” y nos mostrará la URL de nuestra rama Master para poder clonarlo. Copiamos la URL.

![image](https://user-images.githubusercontent.com/89370556/164998805-4034025c-3e47-4641-8ba7-b97c7feeb06d.png)

Buscamos una ruta local donde será clonada la rama del repositorio. Click derecho y seleccionamos la opción “Git Bash Here” (es importante tener Git Instalado para que nos muestre dicha opción) y se nos mostrará una consola.

![image](https://user-images.githubusercontent.com/89370556/164998814-335766d4-885a-4fe1-a685-866fd722dffa.png)

Finalmente, dentro de la consola escribimos el siguiente comando “git clone” + “url copiado del repositorio” + Enter.

`$ git clone <URL>`

![image](https://user-images.githubusercontent.com/89370556/164998856-26804925-4161-4619-89eb-a3db8889fe8b.png)

![image](https://user-images.githubusercontent.com/89370556/164998859-875e87cb-e72e-44ab-84d7-f244bad8af6d.png)

![image](https://user-images.githubusercontent.com/89370556/164998864-2cd85b9d-fa27-4500-8adc-1ba8787d35ea.png)

## Ve el estado de tus archivos con GIT STATUS

El comando Git Status nos informará sobre la rama en la que se está trabajando.

¿Qué tipo de información podemos obtener con el comando Git Status?

- Nuevos archivos creados, modificados y/o eliminados.
- Comandos pendientes, ya sea de envío o de recibo (git pull).
- Rama actualizada.

Veamos un ejemplo de cómo funciona Git Status en la práctica.

Ingresamos a la carpeta que acabamos de clonar, click derecho git bash here.

![image](https://user-images.githubusercontent.com/89370556/164998934-d436d768-16c1-4a62-8249-437c65369cd6.png)

Una vez dentro de la consola escribimos el siguiente comando:

`$ git status`

![image](https://user-images.githubusercontent.com/89370556/164998951-286be3a7-019c-4daf-8972-737b7b100411.png)

La consola nos muestra el mensaje “On branch master Your branch is up to date with ‘origin/master”, eso significa que nuestra rama se encuentra actualizada con el origen.

En este caso vamos a abrir el proyecto para modificar cualquier archivo y volver a ejecutar el comando git status.

Modificaremos el archivo llamado CatalogoController.

![image](https://user-images.githubusercontent.com/89370556/164998987-5ed1dfeb-ba10-46f5-a58e-5733c8f00c25.png)

![image](https://user-images.githubusercontent.com/89370556/164998992-d6d380b3-1d5c-4a22-b614-e51bb795a93d.png)

Tras haber guardado los cambios del archivo con control + s , volvemos a la consola y escribimos nuevamente git status.

![image](https://user-images.githubusercontent.com/89370556/164999000-56aa60cf-2820-432b-8e00-6fb57321a381.png)

Como se puede apreciar, se muestra el archivo que se acaba de modificar, por otro lado, se está listando archivos adicionales de configuración sin haberlos modificado por nosotros mismos, eso sucede porque no hemos creado el archivo git.ignore que le ordena a Git las carpetas o archivos que deberá ignorar de nuestro proyecto. Dicho archivo, se deberá ubicar en el directorio raíz del proyecto.

## Incluye tus nuevos cambios con el comando GIT ADD

Tenemos claro que al momento de realizar cambios en nuestro proyecto, el comando git status nos muestra una lista de todos los archivos que hemos modificado, los cambios solo aparecen en nuestro proyecto local y no se incluirán en el siguiente commit que realicemos.

Si deseamos incluir nuestros cambios en el siguiente commit, usaremos el comando git add, lo podemos hacer tanto para un archivo especifico o para todos los archivos.

Continuando con nuestro ejemplo anterior, podemos observar que los archivos modificados pueden ser incluidos en el siguiente commit con el comando git add.

![image](https://user-images.githubusercontent.com/89370556/164999023-76ab9dab-c6b1-46df-8f80-80113ad2e64b.png)

Si escribimos el comando git add . ocurrirá lo siguiente:

`$ git add .`

![image](https://user-images.githubusercontent.com/89370556/164999040-2dff982d-142a-4724-b843-ab3459127d25.png)

Si escribimos git status nos mostrará todos los archivos que podrán ser incluidos en nuestro siguiente commit

![image](https://user-images.githubusercontent.com/89370556/164999046-d816db3b-5c4f-4326-acb5-4c4ae1fa98ca.png)

Recuerda:
Si deseamos añadir un único archivo usaremos git add <archivo>, si deseamos añadir todos usaremos git add.
  
## Revierte tus cambios con GIT REVERT

En algunos casos vamos a necesitar revertir algunos cambios que hemos hecho. Si bien hay muchas formas de revertir nuestros cambios, en cuanto a comandos git básicos se refiere, git revert es el más popular por los desarrolladores. Antes de ejecutar el comando git revert, necesitaremos saber el historial de los commits, para ello usaremos el comando git log –oneline

`$ git log --oneline`
  
  ![image](https://user-images.githubusercontent.com/89370556/164999078-2b1e9c2d-2bbb-446a-a841-d5b897b7e169.png)

Una vez teniendo el historial, debemos de seleccionar el id de un commit para poder revertirlo:

![image](https://user-images.githubusercontent.com/89370556/164999132-4964a630-71d5-49aa-92e4-cbd9f215b007.png)

Al deshacer un commit con git revert, se creará un nuevo commit. Para poder ver el commit, ejecutaremos el comando git log –branches –not –remotes
  
`$ git log --branches --not --remotes`
 
 ![image](https://user-images.githubusercontent.com/89370556/164999153-6aa26e4b-b199-491b-84b7-e03b6c63ae0a.png)
  
La ventaja principal del comando git revert es que todo sucederá en nuestro local (a no ser que lo enviemos al servidor remoto). Por tal razón el comando git revert es el más usado al momento de revertir nuestros cambios no deseados.

## El comando más popular GIT COMMIT

Si nos referimos a comandos Git, posiblemente el que viene a continuación sea el más popular y usado en este entorno. Git commit es el comando que nos permitirá guardar nuestros cambios en el repositorio actual. Es recomendable usar el comando Git Commit junto con un mensaje para que el equipo de desarrollo sepa el porque de nuestra creación, modificación o eliminación de los archivos que incluyen el commit. Veamos un ejemplo:

En nuestro ejemplo anterior, observamos que al momento de ejecutar git add . todos nuestros archivos estaban listos para ser guardados con el comando git commit.

La forma más común es escribir git commit, pero como bien mencionamos es recomendable realizar el git commit junto con un mensaje, para ello escribimos git commit -m ‘ Mensaje del commit‘

`$ git commit -m 'Mensaje del commit'`
  
![image](https://user-images.githubusercontent.com/89370556/164999232-ba669775-3fa3-43e6-a10d-11b1f7f0698f.png)

Como se puede ver en la imagen, el mensaje del commit es “Commit para el blog de Steven Lizarzaburu Pezúa” . No olvides que cualquier archivo que hayas creado, modificado o eliminado y que no hayas hecho el respectivo git add previamente, dichos archivos no serán guardados con el comando git commit, solo se mantendrán en el disco local, por ello siempre es recomendable ejecutar un git status previo al git commit. Si ejecutamos nuevamente el comando git status, podremos observar que la consola nos muestra el siguiente mensaje:

“On branch master Your branch is ahead of ‘origin/master’ by 1 commit”

El mensaje significa que tenemos 1 commit pendiente para enviar a nuestro servidor remoto (en este caso github). Recuerda que git add y git commit son operaciones que funcionan de manera local. git push, git pull y git fetch son operaciones que funcionan a distancia.

## Fusiona tus ramas con el comando GIT MERGE

Supongamos que tenemos 3 ramas en nuestro repositorio llamadas: dev, test y master. Por lo habitual al inicio se suele trabajar en la rama dev con el equipo, tras haber validado toda la rama de dev y todos los requerimientos correspondientes, dichos cambios deben ser fusionados con la rama test. El comando git merge fusiona todas las características de tu rama actual con la rama que elijas.

`$ git merge <nombre de la rama>`

## Cambia de rama con GIT CHECKOUT

El comando git checkout se suele usar mucho cuando se va a realizar un merge, ya que te permitirá cambiarte de tu rama actual a otra que elijas. Antes de cambiarse a otra rama, se recomienda guardar los cambios de la rama actual en la que se está trabajando.  Git checkout también te permite crear una rama.

Para cambiarte a otra rama usa el siguiente comando:

`$ git checkout <nombre-rama>`

Para crear una rama y cambiarte a ella usa el siguiente comando:

`$ git checkout -b <nombre-rama>`

## Envía tus cambios al servidor remoto con GIT PUSH
  
Ya hemos guardado nuestros cambios con git add y con git commit, ahora falta enviarlo al servidor remoto. El comando git push envia los commits que han sido confirmados al servidor remoto. Antes de escribir el comando git push, se recomienda ver cuales son los commits que se encuentran pendientes. Para ello escribimos el siguiente comando:

`$ git log --branches --not --remotes`

![image](https://user-images.githubusercontent.com/89370556/164999398-81d61949-0a30-478c-a200-f04d83c2c7ca.png)
  
Luego de haber confirmado cuales son nuestros commits pendientes, escribimos el siguiente comando

`$ git push <nombre-remoto> <nombre-de-tu-rama>`

![image](https://user-images.githubusercontent.com/89370556/164999419-0cc68b97-cc25-405e-95b6-c890fc32c44f.png)

Comprobamos nuevamente los commits pendientes  con git log –branches –not –remotes

![image](https://user-images.githubusercontent.com/89370556/164999428-f8b3407e-d046-4f20-a20e-eab744e1ee27.png)

## Obtén cambios y fusiónalos con Git Pull
  
Ya tenemos los comandos necesarios para poder trabajar en equipo, sin embargo ¿Cómo actualizamos los archivos de nuestro proyecto si un miembro del equipo ha enviado nuevos cambios con el comando git push?. El comando git pull nos permitirá actualizar nuestro proyecto local tomando como base el repositorio remoto. En realidad git pull es una combinación del comando git fetch y git merge por lo que significa cuando usemos git pull obtendremos archivos actualizados del repositorio remoto (git fetch) y se fusionarán dichas actualizaciones con nuestro proyecto local (git merge).  Aplicarlo en la practica es muy sencillo.

Dentro de la consola escribimos git pull. Si hay archivos que se deben actualizar la consola nos mostrará los archivos que se han actualizados, de lo contrario si nuestro proyecto se encuentra actualizado, nos mostrará el mensaje ‘Already up to date’.

`$ git pull`
  
![image](https://user-images.githubusercontent.com/89370556/164999452-d1c566be-1eb0-4c6d-996e-6e28ae301b66.png)

Recuerda que GIT cuenta con una larga lista de comandos que te permitirán agilizar el trabajo en equipo, sin embargo es muy poco probable que llegues a usar todos los comandos a la hora de realizar tus proyectos personales.

¡Gracias por leer!. ¡Hasta la próxima!.

# Deployment de Entorno de Producción CI/CD

## MTIE - 501

### Ing. Miguel Manuel Martínez Vázquez

[![Version](https://img.shields.io/badge/Version-1.0.0-green.svg)](https://github.com/djmai/deploy-mtie501/releases/tag/Deploy-CI-CD-v1.0.0)

[![donate](https://www.paypalobjects.com/en_US/i/btn/btn_donate_SM.gif)](https://paypal.me/IngMiguelMartinez?locale.x=es_XC)

_Este proyecto contiene una breve descripción sobre mi persona, y de todos aquellos proyectos que he desarrollado a lo largo de mi carrera de Ingeniera en Tecnologías de la Información y Comunicación en el Area de Sistemas Informáticos_

## Enlaces rápidos

- [Comenzando 🚀](#Comenzando)
  - [Pre-requisitos 📋](#Pre-requisitos)
- [Instalación 🔧](#Instalación)
  - [Ejecución Rápida 🚀](#Speed)
  - [Instalación Docker ⚙️](#Docker)
  - [Ajustando carpetas 🔩](#Ajustando)
- [Despliegue 📦](#Despliegue)
  - [Portal 📦](#Portal)
  - [Angular 📦](#Angular)
  - [Monitor 📦](#Monitor)
  - [Wordpress 📦](#Wordpress)
  - [NodeJSApi 📦](#NodeJSApi)
  - [ApiNetCore 📦](#ApiNetCore)
- [Construido con 🛠️](#Construido)
- [Contribuyendo 🖇️](#Contribuyendo)
- [Wiki 📖](#Wiki)
- [Versionado 📌](#Versionado)
- [Autores ✒️](#Autores)
- [Licencia 📄](#Licencia)
- [Expresiones de Gratitud 🎁](#Gratitud)

<a name="Comenzando" />

## Comenzando 🚀

Como obtener una copia del repositorio completo para trabajar de forma local si te agrada lo que he desarrollado

Para crear la carpeta de `deploy-mtie501` e instalar los requerimientos sólo clona el repo:

```bash
# Clona el repo desde tu terminal:
> git clone https://github.com/djmai/deploy-mtie501.git
```

```bash
# Clona el repo desde Github Desktop (Windows):
1. Inicia sesión en GitHub y GitHub Desktop antes de comenzar la clonación.

2. En GitHub, visita la página principal del repositorio.

3. Sobre la lista de archivos, da clic en  Código.

4. Clic en Open with GitHub Desktop para clonar y abrir el repositorio con with GitHub Desktop.

5. Haz clic en Choose... (Elegir...) y, a través de Windows Explorer, desplázate hasta la ruta donde deseas clonar el repositorio.

6. El botón Clone (Clonar)
```

Mira **Programador** para conocer como desplegar el proyecto.

<a name="Pre-requisitos" />

### Pre-requisitos 📋

_Para poder desplegar el proyecto ocuparemos lo siguiente_

```bash
- Sistema Operativo VM
  - Ubuntu Server 18.04 x64
  - Memoria RAM 2GB Mínimo
  - Disco Duro 80GB Mínimo
  - Procesador 2 NÚcleos

- Software
  - Docker
  - Docker Compose

```

<a name="Instalación" />

## Instalación 🔧

<a name="Speed" />

### Ejecución Rápida

```bash

# Accedemos al a carpeta del proyecto clonado
> cd deploy-mtie501

# Ejecutamos el siguiente comando
> docker-compose -f ./docker-compose.yml up --build -d

```

<a name="Docker" />

### Instalación Docker ⚙️

_Si no tenemos docker y docker compose en nuestro equipo ejecuta lo siguiente_

```bash

# Abrimos una terminal y escribimos lo siguiente
# Recuerda estar dentro de la carpeta de nuestro proyecto deploy-mti501

> sudo sh ./install_docker.sh

```

<a name="Ajustando" />

### Ajustando carpetas 🔩

```bash

# Accedemos a la carpeta de nuestro repositorio clonado

> cd deploy-mtie501

```

```bash

# Opcional
# si quieres ejecutar todo en raíz
# Movemos las siguientes carpetas

> sudo mv src/apinetcore/ ../
> sudo mv src/app-angular/ ../
> sudo mv src/deploy-node/ ../
> sudo mv src/docker-compose.yml ../
> sudo mv src/tartbootstrap-sb-admin-2/ ../
> sudo mv src/README.md ../

```

```bash

# Opcional
# si tienes contenedores y carpetas de src y volúmenes
# usa estos comandos para eliminar dichas carpetas

# Elimina carpeta
> sudo rm -rRf NOMBRE_DE_LA_CARPETA

# Elimina todos los contenedores en ejecución
> docker rm -f $(docker ps -qa)

# Elimina todos las imágenes de docker
> docker rmi -f $(docker images -a -q)

```

<a name="Despliegue" />

## Despliegue 📦

_A continuación te mostramos los accesos para que puedas desplegar las aplicaciones de cada contenedor que desplegamos_

_Abrir el navegador preferido que utilicen y abrir las siguientes urls_

<a name="Portal" />

### Portal

```bash

http://portal.midominiomtie.net

```

<a name="Angular" />

### Angular

```bash

http://angular.midominiomtie.net

```

<a name="Monitor" />

### Monitor

```bash
http://monitor.midominiomtie.net

```

<a name="Wordpress" />

### Wordpress

```bash

http://wordpress.midominiomtie.net

```

<a name="NodeJSApi" />

### Api NodeJS

```bash

http://apinode.midominiomtie.net

```

<a name="ApiNetCore" />

### Api Net Core

```bash

http://apinetcore.midominiomtie.net/WeatherForecast

```

<a name="Construido" />

## Construido con 🛠️

_Utilizamos las siguientes herramientas para desarrollar este proyecto_

- [Docker](https://www.docker.com/) - Plataforma abierta para desarrollar, enviar y ejecutar aplicaciones.
- [Docker Compose](https://docs.docker.com/compose/install/) - Herramienta para definir y ejecutar aplicaciones Docker de varios contenedores.
- [NodeJS](https://nodejs.org/en/) - Entorno en tiempo de ejecución multiplataforma
- [Angular](https://angular.io/) - Framework para aplicaciones web desarrollado en TypeScript
- [Bootstrap’s ](https://getbootstrap.com/) - Framework para hojas de estilo

<a name="Contribuyendo" />

## Contribuyendo 🖇️

Por favor lee el [CONTRIBUTING.md](https://gist.github.com/djmai/deploy-mtie501/CONTRIGUTING.md) para detalles de nuestro código de conducta, y el proceso para enviarnos pull requests.

<a name="Wiki" />

## Wiki 📖

Puedes encontrar mucho más de cómo utilizar este proyecto en nuestra [Wiki](https://github.com/djmai/deploy-mtie501/wiki)

<a name="Versionado" />

## Versionado 📌

Usamos [SemVer](http://semver.org/) para el versionado. Para todas las versiones disponibles, mira los [tags en este repositorio](https://github.com/djmai/deploy-mtie501/tags).

<a name="Autores" />

## Autores ✒️

_Menciona a todos aquellos que ayudaron a levantar el proyecto desde sus inicios_

- **Ing. Miguel Martinez** - [djmai](https://github.com/djmai)

También puedes mirar la lista de todos los [contribuyentes](https://github.com/djmai/deploy-mtie501/CONTRIBUTING.md) quíenes han participado en este proyecto.

<a name="Licencia" />

## Licencia 📄

<a name="Gratitud" />

## Expresiones de Gratitud 🎁

- Comenta a otros sobre este proyecto 📢
- Invita una cerveza 🍺 o un café ☕ a alguien del equipo.
- Da las gracias públicamente 🤓.
- etc.

---

⌨️ con ❤️ por [Ing. Miguel Martinez](https://github.com/djmai) 😊

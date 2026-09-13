# Creación y sincronización de repositorios con Git y GitHub

## Objetivo de la práctica

Creación y sincronización de repositorios con Git y GitHub

Crear un repositorio local utilizando Git, sincronizarlo con un repositorio remoto en GitHub y comprobar el flujo de trabajo en ambos sentidos.

## Descripción del procedimiento realizado

Desde la computadora creamos una carpeta con Powershell dónde pondremos los documentos que queramos guardar y tener en un historial de versiones, ya teniendo esto usaremos GitHub para sincronizar desde ahí un repositorio online que podamos usar para compartir y editar nuestros archivos de forma remota.

## Descripción de los archivos contenidos en el repositorio

1. README.md - archive donde se explica y se da información sobre la práctica realizada (de forma en markdown).

2. datos.txt - nota de documentos para ir practicando y observando cómo funcionan cambia y se interactúa con los archivos en computadora y en línea.

## Comandos de Git utilizados

| # | Comando | Descripción |
|---|---------|-------------|
| 1 | git init | Crea una carpeta oculta y guardará el historial de cambios. |
| 2 | git branch -M main | Renombra la rama actual a main. |
| 3 | git status | Muestra qué archivos han cambiado, cuáles están listos para commit y cuáles se modificaron. |
| 4 | git add . | Sube los archivos modificados y nuevos a staging área. |
| 5 | git commit -m "Primer commit" | Guarda los archivos en un commit, mas un mensaje relacionado |
| 6 | git remote add origin "URL_DEL_REPOSITORIO" | Conecta el repositorio de la computadora con uno remoto en GitHub. |
| 7 | git remote -v | Sirve para confirmar el origin de la URL correcta. |
| 8 | git push -u origin main | Sube por primera vez la rama main al repositorio remoto. |
| 9 | git pull origin main | Descarga los cambios del repositorio remoto y los fusiona con el que está en la compu. |
| 10 | git push | Sube los cambios hechos desde la compu al remoto. |

## Explicación de cómo se creó el repositorio local

Para crear nuestro Repositorio local, abrimos Powershell, creamos una carpeta nueva o abrimos una carpeta, ya dentro del directorio(carpeta escribiremos el comando 'git init' y así estamos por iniciar nuestro repositorio. con 'git status' podemos ver qué archivos tenemos en la carpeta. Así usando 'git add .' o 'git add "nombre del archivo" los mandaremos a una lista de espera (apareciendo en verde) y ya con 'git commit -m "Información para el commit"' será que crearemos una parte del historial, como un primer paso.

## Explicación de cómo se vinculó el repositorio local con GitHub

Para sincronizar el repositorio local con el repositorio remoto, abrimos un repositorio en GitHub y solo lo nombramos sin agregar un contenido extra. Ya creado usaremos 'git remote add origin "URL_DEL_REPOSITORIO"' dentro de nuestra carpeta de la compu (en la parte entre comillas se pone el URL que se nos da en GitHub) t con 'git remote -v' comprobamos que haya salido correctamente la fusión.

## Explicación de la sincronización Local → GitHub

- Al modificarse archivos, hacer otros o eliminar algunos se usa "git push" para cargar todos los commits o modificaciones al repositorio remoto.

## Explicación de la sincronización GitHub → Local

"git pull origin main"

- Cuando se creó, elimino o modifico en el repositorio de remoto, usando "git pull origin main" para descargar esas modificaciones y seguir trabajando.

## Conclusión personal de la práctica

Esta práctica es realmente adecuada para poder empezar a acostumbrarse a lo que es crear un historial de nuestras prácticas y poder compartirlas de una forma más extensa, y directa como lo son los repositorios de GitHub. Sin embargo debo de destacar que puede llegar a ser algo confuso las primeras veces que se usa, pero no le quita que eso mismo sea lo que lo vuelve interesante después y despierta esa curiosidad de pensar que se puede hacer, como funciona y qué más cosas podríamos completar.

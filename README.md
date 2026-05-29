# git practica 2
Taller GIT. Práctica 2.
Guarda los comandos realizados, así como los resultados(capturas), integrarlo dentro del mismo repositorio

## Trabajar con un proyecto HTML y un repositorio local.
- Crea una carpeta practica-taller-git en tu pc.
- Inicializa el repositorio. 
 ```bash
 git init
 ```
<img width="1098" height="618" alt="image" src="https://github.com/user-attachments/assets/d7282431-555c-4096-9663-2c2b9bc4df6e" />

- Crea el fichero index.html con un html simple.
- Comprueba que el repositorio a detectado el cambio. 
```bash
git status
```
<img width="1098" height="617" alt="image" src="https://github.com/user-attachments/assets/bb415f38-61e6-4bdb-8e53-0eebbc23f3a8" />

- Añade el fichero al stage. 
```bash
git add index.html.
```
<img width="1098" height="618" alt="image" src="https://github.com/user-attachments/assets/1ea12fab-84d4-43ec-98f0-76f10c75e831" />

- Confirma los cambios. 
```bash
git commit -m “added index file”
```
- Añade un fichero description.html y edita index.html.
- Comprueba que ha detectado el nuevo fichero y la modificación de index.
```bash
git status
git diff
```
- Crea un fichero TODO.txt de tareas pendientes.
- Comprueba que git ha detectado el nuevo fichero. 
```bash
git status
<img width="1098" height="618" alt="image" src="https://github.com/user-attachments/assets/66549f1d-b8e9-4079-8580-91afea171f90" />

```
- Ignora el fichero TODO.txt ya que es donde anotaremos nuestras tareas personales y no debe formar parte del proyecto. Para ello crea un fichero .gitignore con la linea TODO.txt.
- Comprueba que ya no detecta el nuevo fichero TODO.txt (si que detectara el .gitignore claro). 
```bash
git status
```
<img width="1098" height="617" alt="image" src="https://github.com/user-attachments/assets/4883d06f-7da7-4463-b605-0699ccb1acfd" />

- Añade y confirma el .gitignore.
- Puedes continuar añadiendo ficheros html, css e imágenes para probar el repositorio.


## Haz un fork del repositorio creado para la práctica del taller:
- Entra en https://github.com/
- Accede a tu cuenta.
- Accede al repositorio del profesor https://github.com/lalobarri/git-practica-2.git
- Pulsa el botón fork (parte superior derecha) para crearte una copia del mismo en tu cuenta.
- Clona el repositorio en tu equipo *en otra carpeta diferente que la llamaremos 'git-practica-2'*. Quedará algo parecido a lo siguiente:
```bash
git clone https://github.com/[tu-nombre-de-usuario]/git-practica-2.git
```
- Crea un nuevo fichero en el proyecto que se llame [tu-nombre-de-usuario].html
- Edita el fichero añadiendo como título tu nombre, algún texto y lo que desees en el.
- Añade el fichero al repositorio.
- Súbelo al repositorio remoto (github). 
```bash
git push
```
- Crea una rama develop y cámbiate a ella.
```bash
git checkout -b develop
```
- Realiza cambios en el proyecto, confírmalos y súbelos al repositorio remoto.
```bash
git status
git add *
git commit -m "Mensaje del commit..."
git push origin
```
- Desde github crea un pull request de la rama develop a main.
- Fusiona la rama develop con en main. No deberías de tener ningún conflicto.
- Haz nuevos cambios en el proyecto siguiendo el flujo de trabajo git flow.


## Preguntas
Crea un nuevo fichero respuestas.md, contesta las siguientes preguntas y súbelo a tu repositorio remoto de github:
# RESPUESTAS - PRÁCTICA 2 GIT

---

## 1. ¿Qué sucede cuando hacemos un git add?
Cuando hacemos `git add`, los cambios del archivo se pasan al área de preparación (staging area), donde Git los deja listos para ser confirmados en un commit.

---

## 2. ¿Qué sucede cuando hacemos un git commit? ¿Dónde está ese commit?
Cuando hacemos `git commit`, se guarda una versión del proyecto en el repositorio local dentro de la carpeta oculta `.git`. Ese commit queda almacenado en el historial del proyecto.

---

## 3. ¿Por qué al hacer git commit todavía no está disponible ese commit en el repositorio remoto?
Porque el commit solo existe en el repositorio local. Para que aparezca en GitHub es necesario enviarlo con `git push`.

---

## 4. ¿Qué hay que hacer para que veamos este commit en nuestro repositorio remoto de github?
Se debe ejecutar el comando:
git push

---

## 5. ¿Qué diferencia hay entre hacer un fork o crear una nueva rama?
Un fork crea una copia completa del repositorio en tu cuenta de GitHub.
Una rama solo crea una línea de desarrollo dentro del mismo repositorio.

---

## 6. ¿Qué comando se utiliza para crear una nueva rama sin cambiarte a ella?
El comando es:
git branch nombre-rama

---

## 7. ¿Cuál es la diferencia entre git switch y git checkout?
- `git switch` se usa solo para cambiar entre ramas de forma más moderna y simple.
- `git checkout` es más antiguo y sirve tanto para cambiar ramas como para restaurar archivos.

---

## 8. ¿Qué es una rama por defecto (como main o master) y por qué es importante?
Es la rama principal del proyecto donde se guarda la versión estable del código. Es importante porque sirve como base del desarrollo.

---

## 9. ¿Qué comando te permite ver la lista de todas las ramas locales?
El comando es:
git branch

---

## 10. ¿Qué es una rama (branch) y cuál es su beneficio principal?
Una rama es una línea independiente de desarrollo dentro de un proyecto.
Su beneficio principal es permitir trabajar en nuevas funciones o cambios sin afectar la versión principal del proyecto.

---

## 11. ¿Qué ha pasado con la carpeta practica-taller-git? ¿Por qué no la vemos en GitHub?
La carpeta no aparece en GitHub porque es un repositorio local. Solo se suben los archivos que han sido agregados, confirmados y enviados con `git push`. La carpeta existe en la computadora, pero no se sube automáticamente al repositorio remoto.

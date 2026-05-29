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
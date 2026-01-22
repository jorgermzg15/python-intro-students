git init
git add .
git commit -m "Initial commit: add devcontainer and requirements"
git branch -M main
git push -u origin main
# Python Intro — Notebook hands-on lab

Este repositorio contiene un cuaderno Jupyter diseñado como un laboratorio práctico (hands-on) para enseñar los fundamentos de Python a estudiantes.

Archivo principal

- `Introduccion_a_Python_y_Notebooks.ipynb`: Notebook con explicaciones y celdas preparadas para que los alumnos completen durante la práctica.

Objetivo

El notebook está pensado para ser utilizado en sesiones interactivas de enseñanza. Todas las celdas de código han sido convertidas a comentarios `# TODO:` para que los estudiantes implementen los ejercicios durante la clase.

Quick start (devcontainer)

1. Abre la carpeta en VS Code.
2. Cuando se solicite, reabre en el contenedor (o usa la paleta de comandos: Remote-Containers: Reopen in Container).
3. El contenedor ejecutará `./setup_env.sh` para instalar las dependencias listadas en `requirements.txt`.

Haz ejecutable el script de setup (si es necesario):

```bash
chmod +x "./setup_env.sh"
```

Git: push al remoto

```bash
# inicializar si aún no está inicializado
git init
git add .
git commit -m "Initial commit: cleaned notebook for hands-on lab"

# añadir remote y empujar (reemplaza la URL del origin si es necesario)
git remote add origin https://github.com/jorgermzg15/python-intro-students
git branch -M main
git push -u origin main
```

Si el repositorio remoto está vacío, los comandos anteriores crearán la rama `main` y subirán el commit inicial.

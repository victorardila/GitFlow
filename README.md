# `Git Flow` <img src="https://github.com/VictorArdila/VictorArdila/assets/89551043/25d307e3-ef06-41e0-8cb1-a979f4f130ac" alt="GitFlow" width="35" height="35">
Para trabajar con el esquema de mis repositorios lo trabajo asi:
## `Creacion de repositorios`
`Cambiar nombre de ramas al iniciar proyecto`

Inicializa git

```bash
git init
```
Agrego los cambios locales
```bash
git add .
```
Hago el commit
```bash
git commit -m "Creacion de estructura inicial"
```
Creo la rama 
```bash
git branch nombre
```
Reviso que se hay creado correctamente
```bash
git branch 
```
Selecciono la rama dev que ya fue creada
```bash
git checkout nombre
```
Le asigno al repo local la url del repo remoto para sincronizarlo
```bash
git remote add link.git
```
Envio los cambios
```bash
git push origin nombre
```

`Para eliminar un archivo en el repo remoto`
```bash
git rm -r --cached __pycache__
```
```bash
git commit -m "Eliminando __pycache__ del repositorio remoto"
```
```bash
git push origin nombre_de_tu_rama
```
`Cambiar nombre de una rama que se renombro remotamente`

Comandos para ela operacion

```bash
git branch -m doc dev
```
```bash
git fetch origin
```
```bash
git branch -u origin/dev dev
```
```bash
git remote set-head origin -a
```
`Renombrar una rama creada de mi repositorio`

Nota: esta rama ya tiene cambios y puede que hayan mas ramas en el mismo repoitorio
Si la consola arroja un error como este:

remote: This repository moved. Please use the new location:
remote:   https://github.com/Valfonsoardila10/Admin-Pharm-con-BD-Proyecto.git
To https://github.com/VictorArdila/Admin-Pharm-con-BD-Proyecto.git
 ! [remote rejected] main (refusing to delete the current branch: refs/heads/main)
error: failed to push some refs to 'https://github.com/VictorArdila/Admin-Pharm-con-BD-Proyecto.git'

Es porque no se permite eliminar ramas principales del repositorio asi que tendras que cambiar esto en configuracion del repositorio

Pasos:

Ve a tu repositorio en GitHub.
- Haz clic en "Settings" (Configuración).
- En el panel lateral, haz clic en "Branches" (Ramas).
- En la sección "Default branch" (Rama por defecto), cambia la rama por defecto a una rama diferente, por ejemplo, develop o cualquier otra que tengas disponible

```bash
git checkout old-branch-name
```
```bash
git branch -m new-branch-name
```
```bash
git push origin --delete old-branch-name
```
```bash
git push origin -u new-branch-name
```
```bash
git branch -d doc
```




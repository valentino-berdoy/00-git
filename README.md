# 00-git
# Primeros pasos con git

## Comandos
```bash
git init    #inicio el proyecto de git (1 sola)

git status        #me muestra el estado actual del trabajo

    #cree/modifiqué el archivo ejem.txt

git add ejem.txt     #agrego archivos al proximo commit
git add .            #agrega TODOS los archivos (excepto los del .gitignore) al próximo commit

git commit -m "mensaje del commit"        #crea un commit (una versión nueva del programa)


git commit --amend                #permite corregir el último commit SI NO SE SUBIO A LA NUBE


git log            #permite ver el registro de commits (fecha, autor, commit message)

git push    #subo mis nuevos commit a la nube

git clone "url"

git pull #actualiza el repositorio

git checkout -b nombreDelaRama #cambia de rama en el repositorio
                               #hay que hacer git add y git commit -m para crear un commit en esta rama

git checkout RAMA #va hacia la rama que le decis

git difftool Y diff RAMA #permiten mostrar la diferencia entre dos ramas (entre la que estoy parada y otra que mencione)

git merge RAMAQUETRAIGO #trae la rama que seleccione hacia la que estoy parado
```

## .gitignore
Es un archivo que va en la misma carpeta donde arranca el proyecto (ubicación raíz)
Permite aclarar qué archivos quiero que mantenga fuera del control de git
Se pueden usar comodines (*.pdf), una instrucción por línea

## ramas/branches

Una rama me permite trabajar en paralelo al trabajo que ya tenía. Puedo crear todas las ramas que necesite, la rama por defecto se llama `master`
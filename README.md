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

git difftool Y diff RAMA/id #permiten mostrar la diferencia entre dos ramas o con commit (entre la que estoy parada y otra que mencione)(en el caso de los commit necesito usar sus IDs)

git merge RAMAQUETRAIGO #trae la rama que seleccione hacia la que estoy parado

git push --set-upstream origin RAMA #pushea toda la rama al repositorio remoto

git checkout ID #vuelvo a commit anteriores OJO PIBE QUE TOCAS AHI PORQUE TE PODES MANDAR LA MACANA MAS GRANDE DE LA HISTORIA DE GIT



#       ..              ....    ..''...'coddddxkkkkkkkOOOOOkxoldxkkkkkkkc'.......................'...
#   ......              .....,:ldxkxdooxkkkkkOOOOOOOOOOkddooxOOOOOOOOOOOkl::;,',:::;,'...''''''''''''
# ..'',,.               .'';okOkkOOOOOOOOOOOOOOOOOOOOOOo,'..':cxOOOOOOOOOOkkkxdxOOOkdc,''''''''''''''
#',;;;;'.           ....',cxkkkkOOOOOOOOOOOOOOOOOOOOkxddddl,...lOOOOOOOOOOOOOOOOOOOOOkl,'',,,,,,,,,,,
#;;;;;;.         .:odxdoodkkkkOOOOOOOOOOOOOOOOOOOkdoodxkxxxddl'cOOOOOOOOOOOOOOOOOOOOOOxol:,,,,,,,,,,,
#;;;;;;'.       ;dOOOOOOOOOOOOOOOOOOOOOOOOOOOOkdokOkxkOOxxOOo;'lOOOOOOOOOOOOOOOOOOOOOOOOOko:,,,,,;;;,
#;;;;;;,.     .;dOOOOOOOOOOOOOOOOOOOOOOOOOOOOkoclkxlodOXOxOd,.;xOOOOOOOOOOOOOOOOOOOOOOOOOOOxoc:;;;;;;
#;;;;;;,.   .:dxkOOOOOOOOOOOOOOOOOOOkxxkOOOkkdldkxoccldkdxkxc;oOOOOOOOOOOOOOOOOOOOOOOOOOOOOkkkkdl:;;;
#c::;;;,'..'ckOOOOOOOOOOOOOOOOOOOOOOxoodkOxoodddxxxdddxxkkkxddkOOOOOOOOOOOOOOOOOOOOOOOOOOOOOkOOOkl::;
#lll:,;:lodkOOOOOOOOOOOOOOOOOOOOOkxdoldodOkxxxxdl;;;:::cdOOxodOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOkOkxdl:
#oooolldkkkOOOOOOOOOOOOOOOOOOOOOOxoccoxddkOOOOOd:'.....;okxxooOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOko
#ooooodxkkOOOOOOOOOOOOOOOOOOOOOOOOdoddkdcokOOOk:..;;'..;c:,. .oOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOx
#;;;;cdkkkOOOOOOOOOOOOOOOOOOOOOOOOkc;:;'..cOOo,..::,. .;;..   .dOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOd
#,;;;:dkkkOOOOOOOOOOOOOOOOOOOOOOOOOc.     .,;..'xKXN0doOk;.    ,x0OOOOOOOOOOOOOOOOOOOOOOO000OOOOOOOko
#;;;;cxkkkkOOOOOOOOOOOOOOOOOOOOOOOOkc.         :KXXNN0dl:.      ;k0OOOOOOOOOOOOOOOOOOOOOO000OOOOOOOOx
#;;;:oxkkkOOOOOOOOOOOOOOOOOOOOOOOOOOOl.        oKKNNXd.         .lOOOOOOOOOOOOOOOOOOOOO00000OOOOOOOOk
#,;cdxkkOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOd,      ,kKXNNk'           .dOOOOOOOOOOOOOOOOOOOOO00OOOOOOOOOOO
#.cdxkkOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOdcc:..kXKNXOc             :OOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOO
#.lxxkkkOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOO00O: :KKXNOl'             cOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOO
#.;dxxkkkOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOO0o. c00KXd'.             cOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOk
# .cxkkkkOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOl. .',,,.               ,kOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOk
#..;dkkkkOOOOOOOOOOOOOOOOOkkOOOOOOOOOOOOOOkl......                'xOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOx
#..cxkkkkOOOOOOOOOOOkkkOOOOOOOkkkOOOOOOOOOOk;            .:;,,.   'xOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOd
#.,dkkkkkkkOOOOOOOOOkkkkOkkkOOkkkOOOOOOOOOOOd.           ;O00Oc   'xOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOkl
#.,dkkkkkkkkkOOkkkkkkkkkOkkkOOkkkkkkkkOOOOOOOc           ,xkOx,   'xOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOkc
#..;oxxxxxkkxkkkxxkkkkkkkkkkkkkkkkkkkxddxkkkOc.           .','.   ,xkkkkkkkkkkkkkkkkkkkkkkkkkkkOOOOd,
#....,codl:odlcodddododl:dddloccdoddxo:lo:coo,.;::;.,;;:;;::::'.;:collloo:loo:cdooocodddddxooolxOOx:.
#.....'oOl,o0xcdkkxokOOl,xkdoo,ckxOkkdodd;;dd;'xOOdcodxOxoxkxkc'ddllcoloo:lod;;kddx;oOxkddkxoocdko;..
#....'lodoloddodddoooddolododdlodddddooodoodx:..... ..........  ;lododdddddodoodoodooddddddddddl;....
#....'lxxddxxxxxxxkxxxxxxxxkkxxxxxxxxxxxxkkkkc.                .okdoodkkkxkxxxxkkkxxxxkkxxxxxdc,.....
#...c;,llolllcddxc;dddoodddc:doodxdloddooc;lo;.;oclxc;;.,c:;;:;cddlodoo:cocodxkoddlodl:ddddoolll:....
#..,xc':cdooolkkk:,dkkxdkkk:;oldxkdlxkxdd:,lo:.lOxkOdll':lclokddkdoxkxd;colxkkkoxxooxl;llodoloxkl....
#..........':looollloooodddoooodoodoooooo:..'.   ... .      ....ldddddddddoodddoddooooll;'..'''''....
#...........:olooooddooodlcoollddddddoddd:',;:;',..','',',;,,..;oddclddlcodxoodddoododol:'...........
#..........,kKdloddkOOOxOc:dd:;doxOkkdxOOOOOx00dOo:xxoxkd00OOc,kOOk;cod:,dOKkx00kdxO00Odx:...........
#...........,;,...',;;;:c:coolclcooooloddddddddddolododdoddddolddddoololclc:,,;;;,,,;;;,,'...........
#..........         .....';ldxxxxxxxdxxxxxkkkkOOOOOOOOOOOOOOOkxxdoodkkkdol:;,,;;;;::;;;;;;;:;;;,',;,.
#........            .......':llll:,,;cc;;lxxkkkxxxkkOOkkkkko:'....':c;'',,;,,,,,:c;,,,;,,;;,;;',;,,.
#

```




## .gitignore
Es un archivo que va en la misma carpeta donde arranca el proyecto (ubicación raíz)
Permite aclarar qué archivos quiero que mantenga fuera del control de git
Se pueden usar comodines (*.pdf), una instrucción por línea

## ramas/branches

Una rama me permite trabajar en paralelo al trabajo que ya tenía. Puedo crear todas las ramas que necesite, la rama por defecto se llama `master`
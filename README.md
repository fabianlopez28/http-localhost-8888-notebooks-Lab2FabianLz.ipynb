# Laboratorio No. 2
## Fabián Arnoldo López Méndez


Click [here]:https://www.youtube.com/watch?v=2sjqTHE0zok&feature=emb_logo

**Git:**
Moldear cada folder, cada comanda. Como se relacionan cada una de ellas. 
Root: 
- Foo 
  - Barxxx
    - "hello world"
- Barxx
  -"git is awesome"

Carpetas a nivel superiores, se les conoce como árboles. Los que siguen, son archivos, estos pueden contener árboles, y así sucesivamente. 
*"Root"* es lo que rastrea el computador. 
La idea es crear varias carpetas (ROOT), y una que nos funcione para revisar cualquier error y corregirla.
También existen los conflictos de confusion: el GIT intentará combinar todas las combinaciones posibles, archivos, etcétera, para que se pueda visualizar.

* ¿Cómo se describe más abajo en la estructura?

•	Type Tree = map { tree | blob }
•	Typpe commit = struct {
Parents array < commit >
Author.String 
Message. String 
Snapshot: tree 
Es un modelo limpio y simple. 

![commit-and-tree]("imágenes/commit-and-tree.png")

* ¿Cómo almacena y aborda datos reales?
•	Type object = blob | tree | commit
Objects = map < string, objects >
Almacenar un objetivo particular. 

Def store (o)
Id = sal (o)
Object[id] = 0
Esta función toma grandes datos y la convierte en una cadena corta a un alto nivel.

Def load (id)
Return object [id]
Es un almacén de direcciones de contenido donde los objetos se direccionan por su hash. 

* Referencias:
Map < string, string >
Todos los comandos que almacena son solo manipulaciones para identificar determinadas referencias. 

Referencia para identificar los archivos en GIT BASH:

fabia@DESKTOP-IKOJEBP MINGW64 ~
$ ds
bash: ds: command not found

fabia@DESKTOP-IKOJEBP MINGW64 ~
$ cd

fabia@DESKTOP-IKOJEBP MINGW64 ~
$ ls
'3D Objects'/
 AppData/
'Application Data'/
'Configuración local'@
 Contacts/
 Cookies@
'Datos de programa'@
 Desktop/
 Documents/
 Downloads/
'Entorno de red'@
 Favorites/
 Impresoras@
 IntelGraphicsProfiles/
'Lab2Fabian.2 Fabián Arnoldo López Méndez'
 Links/
'Menú Inicio'@
 Microsoft/
 MicrosoftEdgeBackups/
'Mis documentos'@
 Music/
 NTUSER.DAT
 NTUSER.DAT{d5e39f1f-638b-11eb-bc4c-dca8628e6203}.TM.blf
 NTUSER.DAT{d5e39f1f-638b-11eb-bc4c-dca8628e6203}.TMContainer00000000000000000001.regtrans-ms
 NTUSER.DAT{d5e39f1f-638b-11eb-bc4c-dca8628e6203}.TMContainer00000000000000000002.regtrans-ms
 OneDrive/
 Plantillas@
 RDP6/
 Reciente@
'Saved Games'/
 Searches/
 SendTo@
 Untitled.ipynb
 Untitled1.ipynb
 Videos/
 anaconda3/
 ntuser.dat.LOG1
 ntuser.dat.LOG2
 ntuser.ini
 source/
 untitled
 untitled1

fabia@DESKTOP-IKOJEBP MINGW64 ~
$ ls .git
ls: cannot access '.git': No such file or directory

fabia@DESKTOP-IKOJEBP MINGW64 ~
$ git.comitt
bash: git.comitt: command not found

La idea del Git Bash es revisar los documentos del computador, pero desde la estructura, por esa razón, los comandos anteriores lo demuestran. Se pueden agregar documentos, archivos, e información desde este software para que el usuario desde su interfaz normal, lo pueda visualizar. 

# Diccionaris
Un diccionari és una estructura de dades complexa que guarda un conjunt de valors format per una parella de **clau - valor**. Molt semblant a un diccionari a la vida real on cada paraula (clau) té un significat (valor).

## Creació d'un diccionari
Podem crear un diccionari inicialitzant el seus valors ...
```
colors_hexadecimals = {"vermell":"#FF0000", "verd":"#00FF00", "blau":"#0000FF"}
print(colors_hexadecimals)
```
Sortida.
```
{'vermell': '#FF0000', 'verd': '#00FF00', 'blau': '#0000FF'}
```
... o un diccionari buit.
```
diccionari = {}
print(diccionari)
```
Sortida.
```
{}
```
## Accés als elements d'un diccionari (*clau*)
Per accedir als valors d'un diccionari utilitzem la seva clau, el primer element de la parella de valors.
```
colors_hexadecimals = {"vermel":"#FF0000", "verd":"#00FF00", "blau":"#0000FF"}
print(colors_hexadecimals["verd"])
``
Sortida.
```
#00FF00
```
## Modificació d'un valor o inserció d'un nou element

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
colors_hexadecimals = {"vermell":"#FF0000", "verd":"#00FF00", "blau":"#0000FF"}
print(colors_hexadecimals["verd"])
```
Sortida.
```
#00FF00
```
## Modificació d'un valor o inserció d'un nou element
La inserció d'un nou element o modificació d'un existent es fa de la mateixa manera. Tot dependrà de si la clau ja existeix o no dins el diccionari.

Afegim un nou element utilitzant una nova clau.
```
colors_hexadecimals = {"vermell":"#FF0000", "verd":"#00FF00", "blau":"#0000FF"}
print(colors_hexadecimals)
colors_hexadecimals["taronja"] = "#FF8000"
print(colors_hexadecimals)
```
Sortida.
```
{'vermell': '#FF0000', 'verd': '#00FF00', 'blau': '#0000FF'}
{'vermell': '#FF0000', 'verd': '#00FF00', 'blau': '#0000FF', 'taronja': '#FF8000'}
```
En canvi, si la clau ja existeix es modificarà el seu valor.
```
colors_hexadecimals = {"vermell":"#FF0000", "verd":"#00FF00", "blau":"#0000FF", "taronja":"#FF8000"}
print(colors_hexadecimals)
colors_hexadecimals["taronja"] = "#F4A020"
print(colors_hexadecimals)
```
Sortida.
```
{'vermell': '#FF0000', 'verd': '#00FF00', 'blau': '#0000FF', 'taronja': '#FF8000'}
{'vermell': '#FF0000', 'verd': '#00FF00', 'blau': '#0000FF', 'taronja': '#F4A020'}
```
## Recorrer un diccionari
Podem utilitzar l'estructura repetitiva *for* per recòrrer i obtenir tots els element d'un diccionari.

La forma bàsica ens retornarà les claus del diccionari.
```
colors_hexadecimals = {"vermell":"#FF0000", "verd":"#00FF00", "blau":"#0000FF", "taronja":"#FF8000"}
for color in colors_hexadecimals:
    print(color)
```
Sortida.
```
vermell
verd
blau
taronja
```
Però podem utilitzar aquestes claus per accedir al diccionari i recuperar els seus valors.
```
colors_hexadecimals = {"vermell":"#FF0000", "verd":"#00FF00", "blau":"#0000FF", "taronja":"#FF8000"}
for color in colors_hexadecimals:
    print(color, "-->", colors_hexadecimals[color])
```
Sortida.
```
vermell --> #FF0000
verd --> #00FF00
blau --> #0000FF
taronja --> #FF8000
```
O podem utilitzar el mètode *items()* per recuperar els dos elements com una tupla de dos elements.
```
colors_hexadecimals = {"vermell":"#FF0000", "verd":"#00FF00", "blau":"#0000FF", "taronja":"#FF8000"}
for color in colors_hexadecimals.items():
    print(color)
```
Sortida.
```
('vermell', '#FF0000')
('verd', '#00FF00')
('blau', '#0000FF')
('taronja', '#FF8000')
```
Donem-li una mica de format al mètode *items()*.
```
colors_hexadecimals = {"vermell":"#FF0000", "verd":"#00FF00", "blau":"#0000FF", "taronja":"#FF8000"}
for clau, valor in colors_hexadecimals.items():
    print(clau, "-->", valor)
```
Sortida.
```
vermell --> #FF0000
verd --> #00FF00
blau --> #0000FF
taronja --> #FF8000
```

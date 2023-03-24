# Llistes
Una llista és una estructura de dades complexa que permet emmagatzemar un conjunt de valors. A diferència d'una variable, on només podem guardar un únic valor, en una llista podem tindra varis valors, del mateix tipus o de tipus diferents.

## Creació d'una llista
Podem crear una llista amb valors ...

```
llista_nombres = [1, 2, 3, 4, 5, 6]
dies_setmana = ["Dilluns", "Dimarts", "Dimecres", "Dijous", "Divendres", "Dissabte", "Diumenge"]
llista_mixta = ['gos', 45, 'barcelona', 7.56, True]
print(llista_nombres)
print(dies_setmana)
print(llista_mixta)
```
Sortida.
```
[1, 2, 3, 4, 5, 6]
['Dilluns', 'Dimarts', 'Dimecres', 'Dijous', 'Divendres', 'Dissabte', 'Diumenge']
['gos', 45, 'barcelona', 7.56, True]
```
... o una llista buida
```
llista = []
print(llista)
```
Sortida.
```
[]
```

## Funció *len()*
Aquesta funció la podem utilitzar amb qualsevol estructura de dades complexa (llista, conjunt, set i diccionari), o fins i tot amb un cadena de caràcters. Ens retornarà un enter indicant el tamany de la lista.
```
llista_nombres = [1, 2 , 3, 4 , 5, 6]
print("La llista_nombres té", len(llista_nombres), "elements")
dia = "Dilluns"
print("L'string dia té", len(dia), "caràcters")
```
Sortida.
```
La llista_nombres té 6 elements
L'string dia té 7 caràcters
```

## Accés als elements d'una llista (*índex*)
Per accedir a un element concret d'una llista s'utilitzen els índexs. Un índex és un nombre enter que indica la posició d'un element dins la llista. El primer element de la llista té l'índex 0.
```
dies_setmana = ["Dilluns", "Dimarts", "Dimecres", "Dijous", "Divendres", "Dissabte", "Diumenge"]
print(dies_setmana[0])
print(dies_setmana[3])
```
Sortida.
```
Dilluns
Dijous
```
### Índex negatius
Podem accedir als elements d'una llista començant per darrera utilitzant índex negatius. El darrer valor tindrà l'índex -1, el penúltim el -2, ...
```
dies_setmana = ["Dilluns", "Dimarts", "Dimecres", "Dijous", "Divendres", "Dissabte", "Diumenge"]
print(dies_setmana[-1])
print(dies_setmana[-3])
```
Sortida.
```
Diumenge
Divendres
```
### Accés a un subconjunt d'elements (*slicing*)
La tècnica de *slicing* ens permet accedir a un subconjunt dels elements de la llista especificant un interval *[inici:final]*. El darrer element serà el que correspon a l'índex *final - 1*.
```
dies_setmana = ["Dilluns", "Dimarts", "Dimecres", "Dijous", "Divendres", "Dissabte", "Diumenge"]
print(dies_setmana[0:3]) # Subconjunt des de l'índex 0 fins el 3 - 1
print(dies_setmana[2:5]) # Subconjunt des de l'índex 2 fins el 5 - 1
```
Sortida.
```
['Dilluns', 'Dimarts', 'Dimecres']
['Dimecres', 'Dijous', 'Divendres']
```
Podem obviar el valor d'inici (per defecte serà un 0).
```
dies_setmana = ["Dilluns", "Dimarts", "Dimecres", "Dijous", "Divendres", "Dissabte", "Diumenge"]
print(dies_setmana[:3]) # Subconjunt des de l'índex 0 fins el 3 - 1
```
Sortida.
```
['Dilluns', 'Dimarts', 'Dimecres']
```
I també podem obviar el valor final (per defecte serà la longitud de la llista, on *longitud -1* correspon al darrer valor)
```
dies_setmana = ["Dilluns", "Dimarts", "Dimecres", "Dijous", "Divendres", "Dissabte", "Diumenge"]
print(dies_setmana[2:]) # Subconjunt des de l'índex 2 fins a 7 - 1
```
Sortida.
```
['Dimecres', 'Dijous', 'Divendres', 'Dissabte', 'Diumenge']
```
Tenim la possibilitat de fer un *slicing* amb índexs negatius.
```
dies_setmana = ["Dilluns", "Dimarts", "Dimecres", "Dijous", "Divendres", "Dissabte", "Diumenge"]
print(dies_setmana[-3:]) # Subconjunt des de l'índex -3 fins al final
```
Sortida.
```
['Divendres', 'Dissabte', 'Diumenge']
```
## Recórrer una llista
Amb l'estructura iterativa *for* podem recórrer una llista i recuperar els seus elements un a un.
```
dies_setmana = ["Dilluns", "Dimarts", "Dimecres", "Dijous", "Divendres", "Dissabte", "Diumenge"]
for dia in dies_setmana:
    print(dia)
```
Sortida.
```
Dilluns
Dimarts
Dimecres
Dijous
Divendres
Dissabte
Diumenge
```
## Mètodes de les llistes
Una llista en Python és un objecte, i els objectes tenen assignats funcions que realitzen accions damunt l'objecte. Aquestes funcions d'un objecte són anomenats **mètodes**. Per utilitzar un mètode s'utilitza l'estructura *objecte.metode()*.

A continuació es descriuen alguns dels mètodes més importants.

**append()**: Afegeix un nou element al final de la llista.
```
mesos = []
mesos.append("gener")
mesos.append("febrer")
print(mesos)
```
Sortida.
```
['gener', 'febrer']
```

**clear()**: Elimina tots els elements de la llista.
```
estacions = ["hivern", "primavera", "estiu", "tardor"]
print(estacions)
estacions.clear()
print(estacions)
```
Sortida.
```
['hivern', 'primavera', 'estiu', 'tardor']
[]
```

**count()**: Retorna el nombre de vegades que es repeteix un element a la llista passat com a paràmetre.
```
fruites = ["poma", "pera", "plàtan", "pera", "kiwi", "pinya", "pera"]
print("Nombre de peres:", fruites.count("pera"))
print("Nombre de kiwis:", fruites.count("kiwi"))
```
Sortida.
```
Nombre de peres: 3
Nombre de kiwis: 1
```

**index()**: Retorna la posició del primer element passat com a paràmetre.
```
fruites = ["poma", "pera", "plàtan", "pera", "kiwi", "pinya", "pera"]
print("Posició de la primera pera", fruites.index("pera"))
print("Posició del primer kiwi:", fruites.index("kiwi"))
```
Sortida.
```
Posició de la primera pera 1
Posició del primer kiwi: 4
```

**insert()**: Insereix un nou element a la llista a la posició indicada com a paràmetre. El mètode conté dos paràmetres, l'índex de la posició on inserir el nou element i el nou element. Els elements de les posicions posteriors es desplaçaran una posició.
```
fruites = ["poma", "pera", "plàtan", "pera", "kiwi", "pinya", "pera"]
print(fruites)
fruites.insert(2, "melò")
print(fruites)
```
Sortida.
```
['poma', 'pera', 'plàtan', 'pera', 'kiwi', 'pinya', 'pera']
['poma', 'pera', 'melò', 'plàtan', 'pera', 'kiwi', 'pinya', 'pera']
```
**pop()**: Elimina l'element que ocupa la posició passada com a paràmetre. Si no s'especifica cap índex s'eliminarà el darrer element.
```
fruites = ["poma", "pera", "plàtan", "pera", "kiwi", "pinya", "pera"]
print(fruites)
fruites.pop(1)
print(fruites)
fruites.pop()
print(fruites)
```
Sortida.
```
['poma', 'pera', 'plàtan', 'pera', 'kiwi', 'pinya', 'pera']
['poma', 'plàtan', 'pera', 'kiwi', 'pinya', 'pera']
['poma', 'plàtan', 'pera', 'kiwi', 'pinya']
```

**remove()**: Elimina element passat com a paràmetre. Si l'element es repeteix, només s'eliminarà el primer.
```
fruites = ["poma", "pera", "plàtan", "pera", "kiwi", "pinya", "pera"]
print(fruites)
fruites.remove("pera")
print(fruites)
```
Sortida.
```
['poma', 'pera', 'plàtan', 'pera', 'kiwi', 'pinya', 'pera']
['poma', 'plàtan', 'pera', 'kiwi', 'pinya', 'pera']
```
Amb una estructura repetitiva i el mètode *count()* podem eliminar tots els elements repetits.
```
fruites = ["poma", "pera", "plàtan", "pera", "kiwi", "pinya", "pera"]
while fruites.count("pera") > 0:
    fruites.remove("pera")
print(fruites)
```
Sortida.
```
['poma', 'plàtan', 'kiwi', 'pinya']
```

**reverse()**: Inverteix la llista.
```
estacions = ["hivern", "primavera", "estiu", "tardor"]
print(estacions)
estacions.reverse()
print(estacions)
```
Sortida.
```
['hivern', 'primavera', 'estiu', 'tardor']
['tardor', 'estiu', 'primavera', 'hivern']
```
**sort()**: Ordena els elements d'una llista. Per defecte els ordenarà de manera ascendent, però amb el paràmetre *reverse* podem fer una ordenació descendent.


Els element de la llista poden ser nombres ...
```
nombres = [4, 7, 1, 3, 9, 2]
print(nombres)
nombres.sort()
print(nombres)
nombres.sort(reverse=True)
print(nombres)
```
Sortida.
```
[4, 7, 1, 3, 9, 2]
[1, 2, 3, 4, 7, 9]
[9, 7, 4, 3, 2, 1]
```
... o cadenes de caràcters.
```
noms = ["Laura", "Joan", "Aina", "Toni", "Marina", "Josep", "Iker", "Joana"]
print(noms)
noms.sort()
print(noms)
```
Sortida.
```
['Laura', 'Joan', 'Aina', 'Toni', 'Marina', 'Josep', 'Iker', 'Joana']
['Aina', 'Iker', 'Joan', 'Joana', 'Josep', 'Laura', 'Marina', 'Toni']
```



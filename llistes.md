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
o una llista buida
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

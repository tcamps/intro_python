# Entrada i sortida bàsica
## Entrada per teclat
Amb la funció *input* podem demanar a l'usuari que introdueixi un text al terminal.
L'entrada de text acabarà quan l'usuari premi la tecla *Enter*.
```
# Demana l'introducció d'un valor a l'usuari el el guarda dins la variable 'un_valor'
un_valor = input()
# Mostra el valor de la variable per pantalla
print(un_valor)
```
**Sortida** (*el primer text correspon al que ha entrat l'usuari i el segon és el resultat del print*)
```
Hola
Hola
```

De manera opcional, podem mostrar un text a l'usuari amb la funció *input*.
```
# Demana el nom a l'usuari i guarda el valor introduït dins la variable 'nom'
nom = input("Introdueix el teu nom: ")
print(nom)
```
**Sortida**
```
Introdueix el teu nom: Toni
Toni
```

El tipus de dades que retorna la funció *input* sempre serà una cadena de text (*string*).
```
nom = input("Introdueix el teu nom: ")
edat = input("Introdueix la teva edat: ")
print(type(nom))
print(type(edat))
```
**Sortida**
```
Introdueix el teu nom: Toni
Introdueix la teva edat: 25
<class 'str'>
<class 'str'>
```

... per explicar ...
funcions int i float
errors que poden produir

funció print
print("", end="")
print(f"{}"



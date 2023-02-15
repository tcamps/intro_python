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
Sortida (*el primer text correspon al que ha entrat l'usuari i el segon és el resultat del print*).
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
Sortida.
```
Introdueix el teu nom: Toni
Toni
```
### Tipus de dades de l'entrada
El tipus de dades que retorna la funció *input* sempre serà una cadena de text (*string*).
```
nom = input("Introdueix el teu nom: ")
edat = input("Introdueix la teva edat: ")
print(type(nom))
print(type(edat))
```
Sortida.
```
Introdueix el teu nom: Toni
Introdueix la teva edat: 25
<class 'str'>
<class 'str'>
```
Si necessitem que les dades entrades per l'usuari siguin nombre podem utilitzar
les funcions *int()* o *float()* per convertir-les.
En el següent codi *entrada* és una cadena de caràcters i amb les dues funcions el convertim 
a enter (*entrada_enter*) i decimal (*entrada_decimal*):
```
entrada = input("Introdueix un nombre: ")
print(type(entrada))
entrada_enter = int(entrada)
print(type(entrada_enter))
entrada_decimal = float(entrada)
print(type(entrada_decimal))
```
Sortida
```
Introdueix un nombre: 5
<class 'str'>
<class 'int'>
<class 'float'>
```
D'aquesta manera ja podem treballar amb nombres i fer operacions.
```
nombre1 = int(input("Introdueix el primer nombre: "))
nombre2 = int(input("Introdueix el segon nombre: "))
suma = nombre1 + nombre2
print("La suma és:", suma)
```
Sortida
```
Introdueix el primer nombre: 5
Introdueix el segon nombre: 10
La suma és: 15
```
Si l'usuari ens introdueix un text que no és un nombre i intentem convertir-lo amb alguna 
de les dues funcions es produirà un error.
Sortida d'exemple del mateix programa de suma anterior (Es produeix un error al aplicar la funció 
*int* al text *6y*):
```
Introdueix el primer nombre: 6y
Traceback (most recent call last):
  File "tutorial.py", line 1, in <module>
    nombre1 = int(input("Introdueix el primer nombre: "))
ValueError: invalid literal for int() with base 10: '6y'
```

## Sortida per pantalla
En aquest punt ja hem vist que podem mostrar informació en el terminal mitjançant la funcio *print*.
A n'aquesta funció li podem passar tantes dades com volgume separades per comes.
```
nom = input("Escriu el teu nom: ")
print("Benvingut al curs", nom, ".", "Espero que t'agradi Python")
```
Sortida.
```
Escriu el teu nom: Toni
Benvingut al curs Toni . Espero que t'agradi Python
```
En l'anterior exemple veure que la funció print rep quatre paràmetres: tres cadenes de text i una variable que conte un valor. La funció *print* mostrarà els paràmetres un a un i separats per un espai.
Podem canviar aquest separador per defecte passant-li un valor al paràmetre *sep*.
```
nom = input("Escriu el teu nom: ")
print("Benvingut al curs", nom, ".", "Espero que t'agradi Python", sep="--")
```
Sortida.
```
Escriu el teu nom: Toni
Benvingut al curs--Toni--.--Espero que t'agradi Python
```
Al final de cada *print* s'insereix un salt de línia. 
```
nom = input("Escriu el teu nom: ")
print("Hola")
print(nom)
```
Sortida.
```
Escriu el teu nom: Toni
Hola
Toni
```
També podem canviar aquesta opció mitjançant el paràmetre *end*.
```
nom = input("Escriu el teu nom: ")
print("Hola", end=" ")
print(nom)
```
Sortida.
```
Escriu el teu nom: Toni
Hola Toni
```
En aquest darrer exemple el primer *print* acaba amb un espai en blanc i el segon amb un salt de línia (opció per defecte).



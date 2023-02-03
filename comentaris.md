# Comentaris
En qualsevol llenguatge de programació, un comentari es correspon en una o varies línies del codi que no seran interpretades o compilades.
Aquestes línies ens poden ser útils per dues coses
1. Afegir explicacions al nostre codi per facilitar el seu entendiment. 
Molt útil per mantenir el codi, ja sigui per nosaltres mateixos o altres programadors.
3. Fer que algunes línies del nostre codi deixen d'interpretar-se. Ens pot ser útil al depurar possibles errors.
## Comentaris d'una sola línia
Es poden crear posant el símbol "#" al principi de la línia. Només es comentarà una línia.
```
# Això és un comentari d'una línia. Aquesta línia no serà interpretada per l'intèrpret de Python
# El següent programa suma dos nombres i mostra el resultat per pantalla.
num1 = 5
num2 = 10
suma = num1 + num2
print(suma)
```
**Sortida**
```
15
```
## Comentaris de varies línies
Es poden comentar varies línies delimitant-les entre tres cometes dobles (*"""*).
"""
Totes les línies entre les tres cometes dobles no seran interpretades per l'intèrpret de Python.
El següent programa suma dos nombres i mostra el resultat per pantalla.
num1 = 5
num2 = 10
suma = num1 + num2
print(suma)
"""
**Sortida**
```
15
```

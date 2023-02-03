# Variables i operadors
## Variables
Una variable és un espai de la memòria principal de l'ordinador, identificat per un nom 
simbòlic on podem guardar informació de forma temporal en els nostres programes.

```
nombre1 = 5
nom = "Python"
```
## Tipus bàsics de dades
Les variables tenen un tipus de dades definit (nombre, text, ...). En Python podem trobar els següents 
tipus de dades:
* Enters (int). Nombres enters positius i negatius: *-2, 0, 4, 10, ...*
* Decimals (float). Nombres reals (decimals) positius i negatius: *3.45, -10,004, ...*
* Booleà (bool). Només poden tindre dos possibles valors: *True o False*.
* Cadena de caràcters *string* (str). Textos alfanumèrics. S'han de limitar entre cometes simples ' ' o dobles " ": *"Hola mon", 'acdefg12345-/_', ...*

Podem veure el tipus d'una variable amb la funció *type* (s'ha utilitzat la funció *print* per treure el resultat per pantalla, més endavant es veurà aquesta funció).
```
nombre1 = 5
nombre2 = 10.67
nom = "Python"
major_edat = True

print(type(nombre1))
print(type(nombre2))
print(type(nom))
print(type(major_edat))
```
**Sortida**.
```
<class 'int'>
<class 'float'>
<class 'str'>
<class 'bool'>
```
## Operadors bàsics
### Operadors aritmètics
Són els que manipulen dades numèriques (enters i reals) i retornen un resultat.
|Operador|Descripció|Exemple|
|:--------:|:----------|:-------|
|+|Suma dos nombres|5 + 6 = 11|
|-|Resta dos nombres|10 - 3.4 = 6.6|
|\*|Multiplica dos nombres|4 * 3 = 12|
|/|Divideix dos nombres|10 / 4 = 2.5|
|//|Divideix dos nombres i retorna un enter no arrodonit (només treu els decimals)|10 // 4 = 2|
|%|Retorna el mòdul (resta d'una divisió) entre dos operadors|10 % 4 = 2|
|\*\*|Retorna la potència entre dos nombres, on el primer és la base i el segon l'exponent|2 ** 3 = 8|

### Operadors relacionals
Comparen dos valors i retornen un booleà (*True o False*).
|Operador|Descripció|Exemple|
|:--------:|:----------|:-------|
|>|Retorna True si el primer valor és major que el segon|10 > 9|
|<|Retorna True si el primer valor és menor que el segon|10 < 11|
|==|Retorna True si els dos valors són iguals|10 == 10|
|>=|Retorna True si el primer valor és major o igual que el segon|10 >= 9|
|<=|Retorna True si el primer valor és menor o igual que el segon|10 <= 11|
|!=|Retorna True si els dos valors són diferents|10 != 9|

### Operadors lògics
Són utilitzats per combinar dos o més condicions.
|Operador|Descripció|Exemple|
|:--------:|:----------|:-------|
|and|Retorna True si totes les condicions es compleixen|10 > 9 and 10 == 10|
|or|Retorna True si, al mensy, es compleix una de les condicions|10 > 9 or 10 != 10|

**Codi d'exemple**.
```
num1 = 10
num2 = 5
num3 = 20
num4 = 3

suma = num1 + num2
divisio_sense_decimals = num3 // num4
modul_divisio = num3 % num4

print(suma)
print(divisio_sense_decimals)
print(modul_divisio)

print(num1 > num2)
print(num1 <= num2)
print(num1 == num2)
print(num1 != num2)
print(num1 > num2 and num1 > num3)
print(num1 > num2 or num1 > num3)
```
**Sortida**.
```
15
6
2
True
False
False
True
False
True
```






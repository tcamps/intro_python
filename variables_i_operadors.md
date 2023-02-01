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
* Enters (int). Nombres enters positius i negatius: -2, 0, 4, 10, ...
* Decimals (float). Nombres reals (decimals) positius i negatius: 3.45, -10,004, ...
* Booleà (bool). Només poden tindre dos possibles valors: True o False.
* Cadena de caràcters *string* (str). Textos alfanumèrics. S'han de limitar entre cometes simples ' ' o dobles " ": "Hola mon", 'acdefg12345-/_', ...

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
Sortida.
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
|:--------:|----------|-------|
|+|Suma dos nombres|5+6=11|

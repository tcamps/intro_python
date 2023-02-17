# Estructures Iteratives (Repetitives)
Col·loquialment anomenats **bucles**, es tracta d'unes estructures que ens permeten repetir un bloc de codi varis cops. En Python, n'hi ha de dos tipus:
- *while*: repeteix les accions mentres es compleix una condició.
- *for*: repeteix les accions un nombre determinat de cops.

## Estructura *while*
Aquesta estructura repetirà el codi que contingui mentre es compleixi la condició. És útil per quan volem repetir un bloc de codi, però d'entrada desconeixem el nombre de vegades que s'haurà de repetir. Normalment, la condició dependrà d'alguna acció que es produeix dins el bloc de codi a repetir.

El següent codi demana nombres a l'usuari i els va sumant fins que l'usuari introdueix un '0'.
```
suma = 0
nombre_entrada = int(input("Introdueix un nombre: "))
while nombre_entrada != 0:
    # Equivalent a suma = suma + nombre_entrada
    suma += nombre_entrada
    nombre_entrada = int(input("Introdueix un nombre: "))
print("El resultat de la suma és", suma)
```
Sortida.
```
Introdueix un nombre: 2
Introdueix un nombre: 3
Introdueix un nombre: 4
Introdueix un nombre: 7
Introdueix un nombre: 0
El resultat de la suma és 16
```
## Estructura *for*
Amb aquesta estructura podem repetir un bloc de codi un nombre determinat de vegades. Al començar el bucle coneixem el nombre de vegades a repetir-lo. Pot ser que coneguem aquest nombre en el moment de programar l'algorisme o durant l'execució (tenim el valor en una variable).

En Python, per utilitzar el bucle *for* necesitem la funció *range*. Tenim tres maneres de cridar a aquesta funció:
1. *range(inici, final, increment)*. Per exemple *range(1, 11, 1)* començarà el bucle en el valor '1', acabarà en el '10' (l'anterior a final) i anirà incrementant d'un a un.
2. *range(inici, final)*. El mateix exemple d'abans seria *range(1, 11)*. Increment agafa el valor '1' per defecte.
3. *range(final)*. Per exemple *range(10)* començarà el bucle en el valor '0' (valor per defecte d'inici), acabarà en el valor '9' i incrementarà d'un en un.

Un exemple complet amb les tres opcions.
```
print("Versió completa de range:")
for i in range(1, 11, 1):
    print(i)

print("Versió amb increment per defecte:")
for i in range(1, 11):
    print(i)
    
print("Versió amb inici i increment per defecte:")
for i in range(10):
    print(i)
```
Sortida.
```
Versió completa de range:
1
2
3
4
5
6
7
8
9
10
Versió amb increment per defecte:
1
2
3
4
5
6
7
8
9
10
Versió amb inici i increment per defecte:
0
1
2
3
4
5
6
7
8
9
```

## Bucles infinits

### Sentència *continue*

### Sentència *break*

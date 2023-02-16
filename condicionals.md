# Estructures condicionals
També anomenades estructures o sentències de decisió, serveixen per definir una instrucció o grup d'instruccions que s'executaran depenent de si compleixen o no una condició.
## Sentència *if*
L'estructura bàsica està formada per la sentència *if*.
```
num1 = 5
num2 = 4
if num1 == num2:
    print("Són iguals")
```
El codi anterior no produirà cap sortida, ja que al no complir-se la condició no s'executarà el codi que la segueix.
## Sagnat (*Identation*)
És important tindre molt clar l'estructura. Després de la condició s'han introduït dos punts ":" i tot el codi de les següents línies només s'executaran si es compleix la condició. Podriem dir que tot el que està dins el *if* és un bloc de codi. En Python, per indicar els blocs de codi s'utilitza el sagnat (*identation*). Hi ha dues maneres de fer aquest sagnat:
- Espais. Com a mínim el codi que volem sagnar ha de tindre un espai. Tot el codi que forma el mateix bloc ha de començar amb el mateix nombre d'espais.
- Tabulació. S'utilitza la tecla tabulació del teclat. **Opció recomenada**.
## Sentència *else*
Amb *else* podem indicar un codi alternatiu a executar si no es compleix la condició.
```
num1 = 5
num2 = 4
if num1 == num2:
    print("Són iguals")
else:
    print("No són iguals")
```
Sortida.
```
No són iguals
```
## Sentència  *elif*
Amb *elif* podem anar fent condicions alternatives si no es compleix l'anterior (sigui un *if* o un *elif* previ). En el moment en que es compleix la condició del *if* o d'un *elif* el programa ja no segueix amb la resta comprovacions. Es pot acabar amb un *else* final amb el codi a exectuar si no es compleix cap condició del *if* i *elif*.
```
nombre = 3
if nombre < 0:
    print("És negatiu")
elif nombre == 0:
    print("Es zero")
else:
    print("Es positiu")
```
Sortida.
```
Es positiu
```
## Sentències *if* anidades
Es poden anidar sentencies *if* dins altres sentències *if*, *elif* o *else*.
```num = 11
if num > 0:
    if num > 10:
        print("És positiu i major que 10")
    else:
        print("És positiu i menor o igual que 10")
elif num == 0:
    print("És zero")
else:
    print("És negatiu")
```
Sortida.
```
És positiu i major que 10
```
## Sentències amb vàries condicions
Dins una mateixa sentència *if* es poden combinar vàries condicions amb *and* o *or*. En el cas de *and* s'han de complir totes les condicions i amb *or* una d'elles.
```
num = 9
if num >= 0 and num <= 10:
    print("És un nombre entre 0 i 10")
else:
    print("No és un nombre entre 0 i 10")
```
Sortida.
```
És un nombre entre 0 i 10
```

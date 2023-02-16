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



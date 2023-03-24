# Funcions
Una funció és un bloc de codi al qual podem cridar pel seu nom i executa una sèrie d'instruccions. Una funció pot rebre paràmetres, valors amb els quals treballa i pot acabar retornant un valor. Els principals objectius de les funcions són els següents:
- Reutilitzar codi. Dins un mateix programa, molts de cops necessitam realitzar una acció que inclou varies instruccions a més d'un lloc. Amb les funcions podem evitar tenir que repetir aquest codi. Creem una funció i la cridem cada cop que ens faixi falta. També podem reutilitzar aquest codi en altres programes. Aquí ja podríem parlar de llibreries i mòduls.
- Organitzar el codi. Quan el nostres programes creixen amb les funcions podem agrupar i organitzar millor el nostre codi.

La funció *print()* és un exemple d'una funció que rep un o varis paràmetres, per exemple els diferents textos que volem mostrar per pantalla. Realitza una acció mostrant els textos per pantalla amb un salt de línia al final i no retorna cap valor.
```
# Li passem dos paràmetres a la funció
# La funció realitza una acció, però no retorna cap valor
print("Hola", "món")
```
Sortida.
```
Hola món
```

La funció *input()* és un altre exemple de funció que pot rebre com a paràmetre un text que es mostrarà per pantalla i retornarà un valor, el text introduït al terminal per l'usuari.
```
# Li passem un paràmetre a la funció
# Com que la funció ens retornarà un valor el guardem dins la variable 'nom'
nom = input("Escriu el teu nom: ")
print("Hola", nom)
```
Sortida.
```
Escriu el teu nom: Toni
Hola Toni
```
La biblioteca estàndard de Python ja incorpora molts de mòduls amb funcions que ens ajuden a desenvolupar els nostres programes. També tenim la possibilitat d'instal·lar noves llibreries. L'índex de paquets de Python és un repositori de programari per Python on podem trobar totes aquestes llibreries: [PyPI](https://pypi.org)
## Creació de les nostres pròpies funcions
Per crear una funció hem d'utilitzar la paraula reservada *def*. Totes les instruccions que formen part de la funció han d'anar indentades. El codi de la funció no s'executarà fins que sigui cridada dins el codi principal.
```
# Definició de la funció
def saluda():
    print("Hola món")
    print("Això és una funció")
    
# Execució de la funció
saluda()
```
Sortida.
```
Hola món
Això és una funció
```
### Paràmetres d'una funció
Al definir la funció, indicarem els paràmetres que ha de rebre. Un paràmetre és com una variable local, només existirà dins la funció.
```
def saluda(nom):
    # Dins la funció existeix la variable 'nom'
    print("Hola", nom)
    print("Benvingut al llenguate Python")
    
nom_persona = input("Com et dius? ")
saluda(nom_persona)
```
Sortida.
```
Com et dius? Toni
Hola Toni
Benvingut al llenguate Python
```
En aquest darrer exemple, la variable *nom_persona* i el paràmetre *nom* no tenen cap relació. *nom_persona* és una variable global que existeix en el codi principal del programa. Al cridar a la funció *saluda* li pasem el valor de *nom_persona* (no la variable) i aquest queda guardat dins la variable local *nom* que només existeix dins la funció.
### Valor de retorn d'una funció
Si volem que la nostra funció retorni un valor utilitzarem la paraula reservada *return*.
```
def suma(nombre1, nombre2):
    resultat = nombre1 + nombre2
    return resultat

num1 = float(input("Introdueix el primer nombre: "))
num2 = float(input("Introdueix el segon nombre: "))
res = suma(num1, num2)
print("El resultat de sumar", num1, "i", num2, "és", res)
```
Sortida.
```
Introdueix el primer nombre: 5
Introdueix el segon nombre: 6
El resultat de sumar 5.0 i 6.0 és 11.0
```
Amb el valor retornat tenim dues opcions:
1. Guardar-lo dins una variable per fer-na un ús posterior. En l'exemple anterior, guardem el resultat de la suma que ens retorna la funció *suma* dins la varialbe *res*.
2. Utilitzar-lo com a paràmetre d'una altra funció. En l'exemple anterior, la cadena de caràcters que ens retorna la funció *input* al demanar cada nombre la passem directament a la funció *float* per convertir-lo a nombre real.

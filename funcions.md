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

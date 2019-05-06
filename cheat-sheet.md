# Cheat-sheet
-------------------------------------
## Syntaxguide

Varje program i python körs från top till botten, om man skriver till exempel
```python
a = 5
a = 3
print(a) # a är 3
```
Är det inte samma sak som att skriva
```python
a = 3
a = 5
print(a) # a är 5
```
En ny rad i python är som ett nytt kommando till datorn. Man kan inte sätta två kommandon på samma rad, och det ska alltid vara minst en nyrad emellan varje kommando.

`#` : Kommentar. Datorn hoppar över allting efter ett `#`, tills det blir en ny rad.

Det är alltid en bra ide att kommentera sin kod, och beskriva vad den gör i stora drag, särskilt saker som inte är uppenbara genom att kolla på koden

## Funktionsanrop:
Funktioner anropas med paranteser`()`. Man kan ge argument till en funktion genom att skriva det i paranteserna, med ett komma emellan varje argument:
`funktion(1, två, "tre")`

### Användbara funktioner:
```python
print(x)	# Skriver ut värdet av x till skärmen. x kan vara (typ) vad som helst
A = input(B)	# Ställer en fråga. B är frågan och svaret sparas i A
float(x)	# Byter typ på x till float
int(x)		# Byter typ på x till int
str(x)		# Byter typ på x till string
```
## Matematik
```python
=       # Stoppa in värdet till höger i variabeln till vänster (i = 2)
+       # Addition
-       # Subtraktion
*       # Multiplikation
/       # Division
%       # Division, men du får resten av divisionen (var försiktig med negativa tal)
		    5 % 3 = 2, 9 % 2 = 1

**      # Upphöjt till 
		    5**3 = 5 * 5 * 5 = 125

==      # Jämför två värden och kollar om de har samma värde
!=      # Jämför två värden och kollar om de har olika värde
a < b   # Kollar om a är mindre än b 
a > b   # Kollar om a är större än b
a is B  # Kollar om värdet a är av typ B.
```
## Variabler
En variabel är som en liten låda där man kan spara saker, som man kan använda någon annan stans. En variabel kan inte användas om man inte har stoppat in något i den först. Annars blir datorn sur :[

Det finns ett speciellt värde som heter `None`. Om man stoppar in den i en variabel så "tömmer" man den. Alla variabler som man inte har använt innan har det värdet.

### Några exempel på variabler
```python
A = 5		# X blir en int
X = 0.1		# X blir en float
X = "text"	# X blir en string
X = A		# X blir samma som A, alltså 5
```
## Typer	
```python
int	# Ett vanligt heltal, kan INTE innehålla decimaler. Man slänger helt enkelt bort allt efter kommat
float	# Ett flyttal, alltså kan det ha decimaler. Flyttal kan dessutom vara oändliga eller NaN (inte ett tal alls)
str	# Text, t.ex. "hej". Man kan addera strängar, t.ex. "a" + "b" = "ab".
	#	Man kan också multiplicera strängar, t.ex. "a" * 3 = "aaa"
```
## Listor

En lista är som en rad variabler. Man kan välja en variabel från raden, och använda den som en normal variabel. Man kommer åt variabler i listor genom att sätta `[]` efter listans namn. Den första variabeln i en lista kommer man åt med `lista[0]`, Alltså börjar man räkna från noll. För att lägga till något i slutet av en lista skriver man t.ex. `lista.append(0)`. `range` är en funktion som genererar en lista med nummer som går från noll till något tal, t.ex. gör `range(50)` en lista som går från 0 till 50.
```python
lista = range(50)
lista[0]  # 0
lista[25] # 25
lista[0] = 5
lista[5] = 2
lista[0]  # 5
```
## If, else, elif
När man vill att koden ska göra olika saker baserat på något värde eller input eller i stort sett vad som helst så använder man sig av ett **if-statement**. Ett if-statement ser ut så här:
```python
if sak:
	# kod i if-statementen, körs om sak är sann
elif sak2:
	# kod som körs om sak är falskt, men sak2 är sannt
else:
	# kod som körs om sak och sak2 är falskt
```
Den gör olika saker beroende på `sak` och `sak2` i det här fallet. Först så prövas `sak`. Om `sak` är sann, så körs koden i if-blocket, och inget annat. Om `sak` är falskt, så prövas sak2. Om sak2 är sann, så körs koden i elif-blocket, och inget annat. Om `sak2` är falskt, så kör den koden i else-blocket. Else-blocket körs alltså om inget annat if- eller elif-block som hänger ihop med else-blocket har körts.
## Loopar och annat
En loop kör en bit kod flera gånger. En for-loop ser ut så här: 

```python
for i in range(n):
    # kod i loopen…
# kod utanför… 
```

Den kör koden inuti sig själv n gånger, och i är antalet gånger loopen har körts och kan användas i loopen.
En while-loop ser ut så här

```python
while(x):
    # kod i loopen…
# kod utanför… 
```

Den körs medan x är sann, det vill säga `True` eller inte `False`. När man använder något som inte är en bool i en while-loop så castas det till en bool.
## Debugging, eller konsten att fixa sina misstag
Detta är något av det viktigaste att kunna när man programmerar. F

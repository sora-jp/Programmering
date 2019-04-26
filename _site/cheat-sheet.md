# Cheat-sheet
-------------------------------------
## Matematik
```python
=	# Stoppa in värdet till höger i variabeln till vänster (i = 2)
+	# Addition
-	# Subtraktion
*	# Multiplikation
/	# Division
%	# Division, men du får resten av divisionen (var försiktig med negativa tal)
		5 % 3 = 2, 9 % 2 = 1

**	# Upphöjt till 
		(5**3 = 5 * 5 * 5 = 125)

==	# Jämför två värden och kollar om de har samma värde
a is B	# Kollar om värdet a är av typ B.
```
## Typer	
```python
int	# Ett vanligt heltal, kan INTE innehålla decimaler. Man slänger helt enkelt bort allt efter kommat
float	# Ett flyttal, alltså kan det ha decimaler. Flyttal kan dessutom vara oändliga eller NaN (inte ett tal alls)
str	# Text, t.ex. "hej". Man kan addera strängar, t.ex. "a" + "b" = "ab".
	#	Man kan också multiplicera strängar, t.ex. "a" * 3 = "aaa"
```
## Variabel
En variabel är som en liten låda där man kan spara saker, som man kan använda någon annan stans. En variabel kan inte användas om man inte har stoppat in något i den först. Annars blir datorn sur :[

Det finns ett speciellt värde som heter `None`. Om man stoppar in den i en variabel så "tömmer" man den. Alla variabler som man inte har använt innan har det värdet.

### Några exempel på variabler
```python
A = 5		# X blir en int
X = 0.1		# X blir en float
X = "text"	# X blir en string
X = A		# X blir samma som A, alltså 5
```

## Syntaxguide
`#` : Kommentar. Datorn hoppar över allting efter ett `#`, tills det blir en ny rad.

En ny rad i python är som ett nytt kommando till datorn. Man kan inte sätta två kommandon på samma rad, och det ska alltid vara minst en nyrad emellan varje kommando. Ett kommando i python kan vara en tilldelning (med `=` tecknet) eller ett funktionsanrop.

Det är alltid en bra ide att kommentera sin kod, och beskriva vad den gör i stora drag, särskilt saker som inte är uppenbara genom att kolla på koden

## Funktionsanrop:
Funktioner anropas med paranteser`()`. Man kan ge argument till en funktion genom att skriva det i paranteserna, med ett komma emellan varje argument:
`funktion(1, två, "tre")`

## Användbara funktioner:
```python
print(x)	# Skriver ut värdet av x till skärmen. x kan vara (typ) vad som helst
A = input(B)	# Ställer en fråga. B är frågan och svaret sparas i A
float(x)	# Byter typ på x till float
int(x)		# Byter typ på x till int
str(x)		# Byter typ på x till string
```
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

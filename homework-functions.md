# Läxa: Funktioner
En funktion är en bit kod som alla kan komma åt. När man kör den koden så *anropar* man funktionen. När man anropar funktioner kan man ge den värden att jobba med. Dessa kallas för *argument*. Ett argument kan vara i stort sett vad som helst. Funktionen kan också ge ett värde tillbaka. Detta värdet kallas för *retur-värde*. Om man anropar en funktion, så kan man sätta den på i stort sett alla ställen som en variabel kan vara. Till exempel så kan man fråga om någons namn med `namn = input("Vad heter du? ")`. Då sparas svaret som en sträng i `namn`.

## Göra egna funktioner
I python så finns det en massa funktioner inbyggda, men man kan också göra egna funktioner. Det gör man med nyckelordet `def`. När man gör en funktion så skriver man ungefär så här:
```python
def funktionsnamn(argument1, argument2):
	# Här ligger koden i funktionen. Den körs inte som vanligt när man startar programmet,
	# 	utan bara när man anropar funktionen
	
	return argument1 + argument2	# Return används för att ge tillbaka ett värde.
					# Här så adderar vi bara argumenten och ger tillbaka det.

# Här är koden utanför funktionen. Den här koden körs som vanligt när man startar funktionen

print(funktionsnamn("a", "b")		# Skriver ut "ab" till skärmen
print(funktionsnamn(5, 4))		# Skriver ut 9 till skärmen
```

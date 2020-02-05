# Python

## Installatie Python

[Download Python](https://www.python.org/downloads/) en installeer deze. Neem de laatste versie, dit is op dit moment versie 3.8.1.
> Als je op een Mac werkt dan is Python al geinstalleerd als onderdeel van je besturingsysteem. Check in een terminal (Finder > Applications > Utilities > Terminal) welke versie je hebt door `python --version` uit te voeren.


## Installatie VS Code Python extension

In VS Code ga naar de Extensions tab ( <kbd>CTRL</kbd><kbd>+</kbd><kbd>SHIFT</kbd><kbd>+</kbd><kbd>X</kbd> ). Zoek op `python` en installeer de Python Extension van Microsoft.

### Python interpreter instellen in VS Code

1. Open de `Command Palette` via <kbd>CTRL</kbd><kbd>+</kbd><kbd>SHIFT</kbd><kbd>+</kbd><kbd>P</kbd>
2. Type `python` in het zoekveld en selecteer `Python: Select Interpreter`. 
3. Kies de Python versie die je net hebt geinstalleerd.

### Python debugger instellen in VS Code

1. Zorg ervoor dat je in de VS Code explorer ( <kbd>CTRL</kbd><kbd>+</kbd><kbd>SHIFT</kbd><kbd>+</kbd><kbd>E</kbd> ) een python bestand hebt geselecteerd. 
   1. >Als je die niet hebt maak een bestand aan met als extensie `.py`.
2. In VS Code ga naar de Debug tab ( <kbd>CTRL</kbd><kbd>+</kbd><kbd>SHIFT</kbd><kbd>+</kbd><kbd>D</kbd> ). Klik op de `settings` icon bovenaan en kies voor `Python file Debug Python file`. 
3. Als je een leeg python bestand hebt copy/paste dan de onderstaande code in je lege bestand:
```python
def main():
    print("test debug")

if __name__ == '__main__':
  main()
```
> Zet een breakpoint door links van regel number 2 te klikken zodat er een rode stip staat voor de regel `print("test debug)`. Druk daarna op de `play` knop bovenaan de Debug tab. Als het debuggen werkt dan stopt je code met uitvoeren bij regel 2. De regel wordt gehighlight en en de rode stip is veranderd in een stip omlijnt met een pijltje naar rechts. Bovenaan je venster in VS Code zijn 6 icons verschenen, voor nu klik op de `play` knop zodat je programma verder gaat met de uitvoer: Je debugger werkt!
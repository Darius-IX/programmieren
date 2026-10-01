<!-- python -m mkdocs gh-deplo -->

<!-- https://squidfunk.github.io/mkdocs-material/reference/code-blocks/#highlighting-specific-lines-lines -->

# Datentypen

## integer
```java
int alter = 23;
alter = 23.5; // !FEHLER!

int anderesAlter;  // deklariert, ohne dass sie einen Wert hat
anderesAlter = alter * 2;  // anderesAlter bekommt einen Wert
// anderesAlter ist gleich alter (23) mal zwei (also ist anderesAlter jetzt 46)
double halbesAlter = alter / 2;

int raumnummer;  // hier wird sie deklariert
raumnummer = 203;  // hier initialisiert
int hausnummer = 17;  // hier wird deklariert und initialisiert in einem Schritt
```

## double
```java
double temperatur = 21.57;
double regenWahrscheinlichkeit = 0.3;
double ergebnis = temperatur * regenWahrscheinlichkeit;
System.out.println(ergebnis);
```

## boolean
```java
// boolean sind entweder true oder false
boolean aelterAls20 = true;
int zahl = 20;
boolean zahlIst20 = zahl == 20;  // wenn die zahl 20 ist, dann ist zahlIst20 true, ansonsten false
if (aelterAls20  == true) 
{  // ACHTUNG! zwei Gleichzeichen zum vergleichen!
    System.out.println("Du bist älter als 20");
} 
else 
{
    System.out.println("Du bist 20 oder jünger");
}
if (zahlIst20 == true) 
{
    System.out.println("Die zahl ist 20");
} 
else if (zahlIst20 == false) 
{
    System.out.println("Die zahl ist NICHT 20");
} 
else 
{
    System.out.println("! Dieser else-Block sollte nie erreicht werden, da zahlIst20 entweder true oder false ist, es gibt keine andere Möglichkeit");
}
```

## String
```java
String name = "Deik";
String ABC = "abc";
double regenWahrscheinlichkeit = 0.3;
String text = name + " " + ABC + " WSK: " + regenWahrscheinlichkeit;
System.out.println(text);
```
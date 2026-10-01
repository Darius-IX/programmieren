# Funktionen

## eigene Funktionen erstellen

```java

public void act() 
{
    // wichtig: wenn ihr eine Funktion aufruft, denkt an Klammer auf und Klammer zu!
    meineFunktion();
}

// 'public void' muss so geschrieben werden, 
// der Name 'meineFunktion' ist frei wählbar
public void meineFunktion() 
{
    System.out.println("Meine Funktion wurde aufgerufen");
}
```

## Funktionen mit Parametern
```java

public void act() 
{
    doppeltPrinten("Dieser Text wird 2x ausgegeben");
}

// String gibt den Datentypen des Parameters an, 
// text ist ein frei wählbarer Variablenname
public void doppeltPrinten(String text) 
{
    System.out.println(text);
    System.out.println(text);
}
```

## Funktionen mit Rückgabewert
```java

public void act() 
{
    if (wurdeAGedrueckt) {
        System.out.println("A wurde gedrückt");
    }
}

// wir ersetzen 'void' durch den Datentyp des Rückgabewertes:
public boolean wurdeAGedrueckt() 
{
    // hier habt hier schon eine Funktion mit Rückgabewert gesehen: wenn a gedrückt ist, dann ist das Ergebnis von isKeyDown true, ansonsten false
    boolean istAGedrueckt = Greenfoot.isKeyDown("a");
    if (istAGedrueckt == true) 
    {
        return true;
    } else {
        return false;
    }
}

// gleiche Alternative
public boolean wurdeAGedrueckt1() 
{
    boolean istAGedrueckt = Greenfoot.isKeyDown("a");
    return istAGedrueckt;
}

// und noch kürzer
public boolean wurdeAGedrueckt2() 
{
    return Greenfoot.isKeyDown("a");
}
```

## Beispiele
```java
public void act()
{
    int zweimalVier = verdoppeln(4);
    System.out.println(zweimalVier);
}

public int verdoppeln(int zahl) 
{
    int ergebnis = 2 * zahl;
    return ergebnis;
}
```
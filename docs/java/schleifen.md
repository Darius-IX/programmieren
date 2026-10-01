# Schleifen

## while-Schleife
```java
int counter = 0;
while(true) 
{
    counter = counter + 1;
    System.out.println("Counter: " + counter);
    // zählt für immer von 1 hoch, also 
    // Counter: 1
    // Counter: 2
    // Counter: 3
    // Counter: 4
    // ...
}

// Führe etwas 10x aus:
int counter = 0;
while (counter < 10) 
{
    counter = counter + 1;
    System.out.println("Counter: " + counter);
    // Counter: 1, 2, 3, 4..., 8, 9, 10
}
System.out.println("Counter: " + counter);  // hier ist der counter bei 10!
```
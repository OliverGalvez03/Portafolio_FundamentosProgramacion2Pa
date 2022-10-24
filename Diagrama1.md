# Diagrama1
## Ejercicio. Contar del 1 al 10 y sumar los valores
### 1.1 Analisis
Se encesita imprimir la suma de los numeros del 1 al 10, para esto se ocupa de un cuadro de proeso que guarde la variable igualada a 0, seguido de el ciclo en forma de for,while y do while, con el cuadro de proceso en donde se guardara la suma de estos, mas el simbolo de salida con la suma.

### 1.2 Diagrama 
![Alt](https://gyazo.com/2fe57f4ae0a914da282d0e93af07704f.png)
![Alt](https://gyazo.com/fcb4fdcef3028a858a78e72eac263a22.png)
![Alt](https://gyazo.com/b9b88406261928de4e7d6a994e806106.png)

### 1.3 Prueba de escritorio
![Alt](https://gyazo.com/8372e004bd096e4e997f5e1125f1ee7c.png)
![Alt](https://gyazo.com/e79199e9f19d232b21353422fba9c75d.png)
![Alt](https://gyazo.com/a75dae09bd30daecc3981add768d67d5.png)

### 1.4 Codigo
#### For
 ```dart
 void main(List<String> args) {
  int s = 0;
  for (var i = 1; i <= 10; i++) {
    s += i;
  }
  print("La suma de los valores es: $s");
}
```
#### While
```dart
void main(List<String> args) {
  int s = 0, c = 1;

  while (c <= 10) {
    s += c;
    c++;
  }
  print("El resultado de la suma de los valores es:$s");
}
```
#### DoWhile
```dart
void main(List<String> args) {
  int s = 0, c = 1;

  do {
    s += c;
    c++;
  } while (c <= 10);
  print("El resultado de la suma de los valores es:$s");
}
```


### 1.5 Entradas
Ninguna

### 1.6 Salidas
55

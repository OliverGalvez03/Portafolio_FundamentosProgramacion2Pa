# Diagrama 6
## Ejercicio. Almacene en un vector de 10 elementos todos los numeros pares capturados por el teclado.
### Analisis 
Se necesita almacenar los numeros pares capturados, iniciando con un cuadro de proceso para asignar el tamaño del vector, seguido de asignar variables en while y en dowhile, seguido de los ciclos con sus condiciones en las formas, for,while y dowhile, terminando con un simbolo de salida con el valor del vector
## For
### Diagrama
![](https://gyazo.com/1dce4ca8344b601ab4d8b0336e4c902b.png)
### Prueba de escritorio
![](https://gyazo.com/4e431edef09140f14956281576886ce7.png)
### Codigo 
```dart
import 'dart:io';
import 'dart:async';

void main() {
  var array = [];

  for (var i = 0; i <= 10; i++) {
    int n = int.parse(stdin.readLineSync()!);
    if (n % 2 == 0) {
      array.add(n);
      i = i - 1;
    }
  }
  print(array);
}

```
## While
### Diagrama
![](https://gyazo.com/194aeb8a5b786cc74967efc5d4490cf0.png)
### Prueba de escritorio
![](https://gyazo.com/8a94969c9e2baa2ca94df7e1d762f6bc.png)
### Codigo
```dart
import 'dart:io';
import 'dart:async';

void main() {
  var array = [];
  var c = 0;

  while (c <= 10) {
    int n = int.parse(stdin.readLineSync()!);
    c = c + 1;
    if (n % 2 == 0) {
      array.add(n);
      c = c - 1;
    }
  }
  print(array);
}
```
## DoWhile
### Diagrama
![While](https://gyazo.com/16574f4b31b9d232202e308518499881.png)
### Prueba de escritorio
![](https://gyazo.com/d2ad005152ac3d04a62f60151c5e5cc3.png)
### Codigo
```dart
import 'dart:io';
import 'dart:async';

void main() {
  var array = [];
  var c = 0;
  do {
    int n = int.parse(stdin.readLineSync()!);

    if (n % 2 == 0) {
      array.add(n);
      c = c + 1;
    }
  } while (c <= 9);
  print(array);
}
```

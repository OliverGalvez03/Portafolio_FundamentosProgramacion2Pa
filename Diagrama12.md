# Diagrama 12
## Ejercicio. Almacenar en un vector el resultado de una tabla de multiplicar 10 numeros
### Analisis
### Diagrama
![](https://gyazo.com/551f8c6fbaa201dc4df956b3766afb93.png)
### Prueba de escritorio
![](https://gyazo.com/ef832ba2836e91cf5756e8b23de5707d.png)
### Codigo
```dart
import 'dart:io';

void main() {
  var array =[];
  int n =int.parse(stdin.readLineSync()!);
  for (var i=0; i<11; i++) {
    array.add(i);
    array[i] =n*i;
  }
  print('$array');
}

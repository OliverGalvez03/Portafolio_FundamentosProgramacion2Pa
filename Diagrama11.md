# Diagrama 11
## Ejercicio. Obtener la distancia mayor de 2 numeros consecutivos en una lista de 10 vectores
### Analisis
Se quiere obtener la distancia entre dos numeros guardados en una lista de 10 elementos, se necesita capturar 10 numeros para guardarlos en una lista, para sacar la diferencia cada 2 numeros de la lista, y decir cual es el mayor.
### Diagrama
![](https://gyazo.com/bc49529fdaa22d021d3dfee9081f30a9.png)
### Prueba de escritorio 
![](https://gyazo.com/8491a7fb4b9acca6136b86e83eace3a5.png)
### Codigo
```dart
import 'dart:io';

void main() {
  var num = [];
  var d = [];
  var dis = 0;
  var mayor = 0;

  for (var i = 0; i <= 9; i++) {
    int n = int.parse(stdin.readLineSync()!);
    if (n < 0) {
      print('el numero no debe ser negativo');
      i = i--;
    }
    if (n > 0) {
      num.add(n);
    }
  }
  print('los numeros son $num');
  for (var i = 0; i < 9; i++) {
    dis = num[i] - num[i + 1];
    d.add(i);
    if (dis < 0) {
      d[i] = dis * -1;
    }
    if (dis > 0) {
      d[i] = dis;
    }
  }
  print('las distancias son $d');
  for (var i = 0; i < 9; i++) {
    if (mayor < d[i]) {
      mayor = d[i];
    }
  }
  print('la distacia mayor es $mayor');
}

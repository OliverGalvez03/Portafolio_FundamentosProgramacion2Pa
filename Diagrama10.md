# Diagrama 10
## Ejercicio. Capturar 10 numeros enteros positivos en un vector, y decir cual es el mayor
### Analisis
Se necesita capturar 10 numeros enteros positivos y guardarlos en un vector de 10 elementos, que diga igual cual es el numero mayor y el numero menor. 
Para esto se necesita de 1 ciclo para que guarde las variables en los vectores con las condiciones necesarias para poder decir si son positivos, seguido de otros 2 ciclos con sus condiciones, que repitan los numeros guardados en los vectores para poder tener cual numero es mayor y cual menor. 
### Diagrama
![](https://gyazo.com/f6298abf13d4814bece1a9de203fb3ae.png)
### Prueba de escritorio
![](https://gyazo.com/576c2d3425d372c9bdc44df8451d1ca3.png)
### Codigo
````dart
import 'dart:io';

void main() {
  var num = [];
  var mayor = 0;
  var menor = 0;
  for (var i=0; i<=9; i++) {
    int n = int.parse(stdin.readLineSync()!);
    if (n > 0) {
      num.add(n);
      if (n < 0) {
        print('El numero debe ser positivo');
        i =i-1;
      }
    }
  }
  print(num);
  for (var i = 0; i <= 9; i++) {
    if (mayor<num[i]) {
      mayor=num[i];
    }
  }
  print('el numero mayor es $mayor');
  menor =mayor;
  for (var i=0; i<=9; i++) {
    if (menor>num[i]) {
      menor =num[i];
    }
  }
  print('el numero menor es $menor');
}

# Diagrama 7
## Ejercicio. Obtener el promedio de las calificaciones aprobatorias y la cantidad de alumnos reprobados 
### Analisis 
Se quiere obtener el promedio de calificaciones y la cantidad de alumnos reprobados, para esto se ocupa ingresar las calificaciones con un maximo de 15 alumnos, consiguiendolo con un ciclo en for,while y dowhile, para despues establecer las condiciones necesarias para determinar si la calificacion es aprobatoria o reprobatoria, sumandose para sacar el promedio  
## For
### Diagrama
![](https://gyazo.com/9accfb5d64e8da4164a0516b412095f2.png)
### Prueba de escritorio
![](https://gyazo.com/8aa2f26e9a1dbf00ec1689eac4b0b6cd.png)
### Codigo
```dart
import 'dart:io';
import 'dart:async';

void main() {
  double proma = 0;
  var contr = 0;
  double sumaa = 0;
  double conta = 0;
  double cal1 = 0;
  double cal2 = 1;

  for (var i = 1; i <= 15; i++) {
    double c = double.parse(stdin.readLineSync()!);
    if (c > 10) {
      print('la calificacion no puede ser mayor a 10');
      i = i - 1;
    }
    if (c < 0) {
      print('la calificacion no puede ser menor a 0');
      i = i - 1;
    }
    if (c < 6 && c > 0) {
      contr = contr + 1;
    }
    if (c <= 10 && c >= 6) {
      cal1 = c;
      sumaa = sumaa + cal1;
      conta++;
    }
    if (cal1 > cal2) {
      cal2 = cal1;
    }
  }
  proma = sumaa / conta;
  print('el promedio de aprobados es $proma');
  print('la calificacion mas alta es $cal2');
  print('la cantidad de reprobados son $contr');
}
```
## While
### Diagrama
![](https://gyazo.com/635d6fcf9dae754350b0f055336c1513.png)
### Prueba de escritorio
![](https://gyazo.com/248565e2fb8931333b38218e312490d9.png)
### Codigo
```dart
import 'dart:io';
import 'dart:async';

void main() {
  double proma = 0;
  var contr = 0;
  double sumaa = 0;
  double conta = 0;
  double cal1 = 0;
  double cal2 = 1;
  var cont = 0;

  while (cont <= 14) {
    double c = double.parse(stdin.readLineSync()!);
    cont = cont + 1;
    if (c > 10) {
      print('la calificacion no puede ser mayor a 10');
      cont = cont - 1;
    }
    if (c < 0) {
      print('la calificacion no puede ser menor a 0');
      cont = cont - 1;
    }
    if (c < 6 && c > 0) {
      contr = contr + 1;
    }
    if (c <= 10 && c >= 6) {
      cal1 = c;
      sumaa = sumaa + cal1;
      conta++;
    }
    if (cal1 > cal2) {
      cal2 = cal1;
    }
  }

  proma = sumaa / conta;
  print('el promedio de aprobados es $proma');
  print('la calificacion mas alta es $cal2');
  print('la cantidad de reprobados son $contr');
}
```
## DoWhile
### Diagrama
![](https://gyazo.com/2ce3d5e70993e08549447995c26aa22b.png)
### Prueba de escritorio
![](https://gyazo.com/284fef69401c37f5a7032383f0c0600c.png)
### Codigo
```dart
import 'dart:io';
import 'dart:async';

void main() {
  double proma = 0;
  var contr = 0;
  double sumaa = 0;
  double conta = 0;
  double cal1 = 0;
  double cal2 = 1;
  var cont = 0;
  do {
    double c = double.parse(stdin.readLineSync()!);
    cont = cont + 1;
    if (c > 10) {
      print('la calificacion no puede ser mayor a 10');
      cont = cont - 1;
    }
    if (c < 0) {
      print('la calificacion no puede ser menor a 0');
      cont = cont - 1;
    }
    if (c < 6 && c > 0) {
      contr = contr + 1;
    }
    if (c <= 10 && c >= 6) {
      cal1 = c;
      sumaa = sumaa + cal1;
      conta++;
    }
    if (cal1 > cal2) {
      cal2 = cal1;
    }
  } while (cont <= 14);

  proma = sumaa / conta;
  print('el promedio de aprobados es $proma');
  print('la calificacion mas alta es $cal2');
  print('la cantidad de reprobados son $contr');
}
```

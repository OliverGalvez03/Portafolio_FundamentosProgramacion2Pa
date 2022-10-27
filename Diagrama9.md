# Diagrama 9
## Ejercicio. 
Obtener la frecuencia de N calificaciones entre [1,10] indique cantidad de reprobados, cantidad de aprobados, promedio de aprobados y promedio general
### Analisis
## For
### Diagrama
![](https://gyazo.com/47b26ebce7af82090af13eae33dc44a9.png)
### Prueba de escritorio
![](https://gyazo.com/3f5f8af0059e8d33d9e5d8411a25db4f.png)
### Codigo
```dart
import 'dart:io';

void main() {
  var contr = 0;
  var conta = 0;
  var contt = 0;
  double sumag = 0;
  double sumaa = 0;
  double promg = 0;
  double porma = 0;
  var C0 = 0;
  var C1 = 0;
  var C2 = 0;
  var C3 = 0;
  var C4 = 0;
  var C5 = 0;
  var C6 = 0;
  var C7 = 0;
  var C8 = 0;
  var C9 = 0;
  var C10 = 0;

  print('inserta las 10 calificaciones entera positiva, entre 1 y 10');
  for (var i = 0; i <= 9; i++) {
    int c = int.parse(stdin.readLineSync()!);

    if (c > 11) {
      print('La calificacion debe ser menor a 10');
      i = i--;
    }
    if (c < 0) {
      print('la calificacion debe ser mayor a 0');
      i = i--;
    }
    if (c == 0) {
      C0 = C0 + 1;
    }
    if (c == 1) {
      C1 = C1 + 1;
    }
    if (c == 2) {
      C2 = C2 + 1;
    }
    if (c == 3) {
      C3 = C3 + 1;
    }
    if (c == 4) {
      C4 = C4 + 1;
    }
    if (c == 5) {
      C5 = C5 + 1;
    }
    if (c == 6) {
      C6 = C6 + 1;
    }
    if (c == 7) {
      C7 = C7 + 1;
    }
    if (c == 8) {
      C8 = C8 + 1;
    }
    if (c == 9) {
      C9 = C9 + 1;
    }
    if (c == 10) {
      C10 = C10 + 1;
    }
    if (c < 11 && c >= 0) {
      if (c >= 6) {
        conta = conta + 1;
        sumaa = sumaa + c;
      }
      if (c < 6) {
        contr = contr + 1;
      }
      sumag = sumag + c;
    }
  }
  porma = sumaa / conta;
  contt = conta + contr;
  promg = sumag / contt;

  print('La frecuencia de 0 es $C0');
  print('La frecuencia de 1 es $C1');
  print('La frecuencia de 2 es $C2');
  print('La frecuencia de 3 es $C3');
  print('La frecuencia de 4 es $C4');
  print('La frecuencia de 5 es $C5');
  print('La frecuencia de 6 es $C6');
  print('La frecuencia de 7 es $C7');
  print('La frecuencia de 8 es $C8');
  print('La frecuencia de 9 es $C9');
  print('La frecuencia de 10 es $C10');
  print('Cantidad de reprobados $contr');
  print('cantidad de aprovaodos $conta');
  print('promedio general $promg');
  print('promedio aprobados $porma');
}
```
## While
### Diagrama
![](https://gyazo.com/ffcef277c6ee88e6ac21b4b319a138bf.png)
### Prueba de escritorio
![](https://gyazo.com/09b9148a8babaedae5bd6c9358bf7250.png)

## DoWhile
### Diagrama
![](https://gyazo.com/15fa5b6392c70739e281c8723c471973.png)
### Prueba de escritorio
![](https://gyazo.com/09b9148a8babaedae5bd6c9358bf7250.png)

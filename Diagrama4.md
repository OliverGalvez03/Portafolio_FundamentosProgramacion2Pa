# Diagrama 4
## Ejercicio. Almanece los n numeros leidos del teclado en un vector de 10 elementos
### Analisis
Se quiere almacenar en en un vector de 10 elementos los numeros ingresados del teclado, para esto primero se necesita, dar el tamaño del array en un cuadro de proceso, seguido de asignar variables en las formas while y do while. Seguido del ciclo en forma for,while y dowhile, para terminar con el simbolo de salida para imprimir el array.

## For
### Diagrama

### Prueba de escritorio

### Codigo
```dart
import 'dart:io';

//Leer 10 numeros del teclado y ponerlos en una lista.
void main() {
  var arra = new List.filled(10, 0);
  stdout.write("Dame diez numeros\n ");
  stdout.write("----------\n");
  for (var i = 0; i <= 9; i++) {
    String? s = stdin.readLineSync();
    if (s != null) {
      int n = int.parse(s);
      arra[i] = n;
    }
  }
  stdout.write("aqui esta la lista, $arra");
}
```
## While
### Diagrama
![](https://gyazo.com/bf1571dbec9c06b20e7a1798f6c81dc7.png)
### Prueba de escritorio
![](https://gyazo.com/8cc9a6ece4a51f0ab948123c4bacde83.png)
### Codigo
```dart
import 'dart:io';

//Leer 10 numeros del teclado y ponerlos en una lista.
void main() {
  var arra = new List.filled(10, 0);
  stdout.write("Dame diez numeros\n ");
  stdout.write("----------\n");
  int i = 0;
  while (i <= 9) {
    String? s = stdin.readLineSync();
    if (s != null) {
      int ner = int.parse(s);
      arra[i] = ner;
    }
    i++;
  }
  stdout.write("Tu lista es, $arra ");
}
```
## DoWhile
### Diagrama
![](https://gyazo.com/696d65ca93604681dea2342f9cfed83d.png)
### Prueba de escritorio
![](https://gyazo.com/02fc6da58bfdecc8bb5094f1b52e1162.png)
### Codigo
```dart
import 'dart:io';

void main() {
  var arra = new List.filled(10, 0);
  stdout.write("Dame diez numeros\n ");
  stdout.write("----------\n");
  int i = 0;
  do {
    String? s = stdin.readLineSync();
    if (s != null) {
      int n = int.parse(s);
      arra[i] = n;
      i++;
    }
  } while (i <= 9);
  stdout.write("Tu lista es $arra ");
}
```

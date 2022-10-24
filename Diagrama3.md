# Diagrama 3
## Ejercicio. Almacenar en un array el numero n leido del teclado, el tamaño del array es 10
### Analisis 
Se ocupa almacenar en un array cuyo tamaño es 10, los numeros n leidos del teclado
## For
#### Diagrama 
![](https://gyazo.com/05a7bf67edb6cabfa1629623c7537eba.png)
#### Prueba de escritorio
![](https://gyazo.com/7d6353fed7c4b00df48ad42a22ecfa97.png)
#### Codigo
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
#### Diagrama
![](https://gyazo.com/187aa35e98ad8294f1fd0f20bd896e77.png)
#### Prueba de escritorio
![](https://gyazo.com/1fb358afd5e2e0e5c30aa0e1915e1142.png)
#### Codigo
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
#### Diagrama
![](https://gyazo.com/77230060e8f36c21b20b17e1705146ba.png)
#### Prueba de escritorio
![](https://gyazo.com/9ebd974e8ddf9413da80b3c17e6f3bbd.png)
#### Codigo
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

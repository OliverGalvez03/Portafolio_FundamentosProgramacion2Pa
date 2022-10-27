# Diagrama 13
## Ejercicio. escriba el siguiente dibujo
##### * 
##### **
##### ***
##### ****
##### *****

### Analisis 
Se quiere hacer el siguiente dibujo, para esto se necesita de dos ciclos para imprimir los asteriscos.
### Diagrama
![](https://gyazo.com/babc771c08c0d691e2c25974a08fcba3.png)
### Prueba de escritorio
![](https://gyazo.com/2d8c0b75f19966ad21515af564b67d52.png)
### Codigo
```dart
import 'dart:io';

void main() {
  var n =5;
  for (var i=0; i<5; i++) {
    for (var j=0; j<=i; j++) {
      stdout.write('*');
    }
    print('');
  }
}

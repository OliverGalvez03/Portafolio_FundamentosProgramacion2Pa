# Diagrama 5
## Ejercicio. Almacene un contador negativo en un vector, el conteo es de 10 a 0
### Analisis. 
Se necesita un contador negativo en un vector, para esto se ocupa un cuadro de proceso para asignar el vector, seguido de un cuadro de proceso para asignar las variables en los casos de while y dowhile, seguido de los ciclos, en for,while y dowhile. Para terminar con un simbolo de salida de datos. 
## For
### Diagrama
![](https://gyazo.com/74a08b4c570351195ea7bd2057a9871d.png)
### Prueba de escritorio
![](https://gyazo.com/4499c18fd5f9c75b4016c7f8fdbd3338.png)
### Codigo
```dart
void main() {
  var arr = <int>[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
  for (var i = 10; i >= 0; i--) {
    arr[10 - i] = i;
  }
  print(arr);
}//For

```
## While
### Diagrama
![](https://gyazo.com/334acff24a55b7f17383fb4bc10fb73a.png)
### Prueba de escritorio
![](https://gyazo.com/75a6307362ba199af8b41cf8c0c66235.png)
### Codigo 
```dart
void main() {
  var arr = <int>[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
  int c = 10;
  while (c >= 0) {
    arr[10 - c] = c;
    c = c - 1;
  }
  print(arr);
}
```
## DoWhile
### Diagrama 
![](https://gyazo.com/857aaa6bfd2649481cdf0f7f0d2a3823.png)
### Prueba de escritorio
![](https://gyazo.com/4d53a5f92ec68c724feb06b9d1fbaba4.png)
### Codigo
```dart
void main() {
  var arr = <int>[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
  int c = 10;
  do {
    arr[10 - c] = c;
    c = c - 1;
  } while (c >= 0);
  print(arr);
}
```

# Diagrama 2
## Ejercicio. Obtener la suma de los primeros 5 numeros pares
### Analisis
Se necesita obtener la suma de los 5 primeros numeros pares

## For
#### Diagrama
![](https://gyazo.com/1981d6f3bff4032fb2c5a72e5c5d324d.png)
#### Prueba de escritorio
![](https://gyazo.com/e5762a70ca6a6a2c1d7c31552e09a1da.png)
#### Codigo
```dart
void main(List<String> args) {
  int s = 0;
  for (var i = 2; i <= 10; i = i + 2) {
    s = s + i;
  }
  print("resultado de la suma de numeros pares es:$s");
}
```

## While
#### Diagrama 
![](https://gyazo.com/1304e8af4fa7b2fad5df4c5cd7c94cd9.png)
#### Prueba de escritorio
![](https://gyazo.com/972e5b166240fcbddfdb723396ea9508.png)
#### Codigo
```dart
void main(List<String> args) {
  int s = 0, c = 1;
  while (c <= 5) {
    s = s + c * 2;
    c = c + 1;
  }
  print("resultado de la suma de numeros pares:$s");
}
```

## DoWhile
#### Diagrama
![](https://gyazo.com/00afc296a6f6c9a15872dff2ef57c379.png)
#### Prueba de escritorio
![](https://gyazo.com/b61b02cc51ed7b1edede6f8c907e6333.png)
#### Codigo
```dart
void main(List<String> args) {
  int s = 0, c = 1;

  do {
    s = s + c * 2;
    c = c + 1;
  } while (c <= 5);
  print("la suma de numeros pares es:$s");
}
```

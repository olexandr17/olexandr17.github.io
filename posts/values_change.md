[Main](/index.md)

## Как поменять значения двух переменных без использования третьей

Вариант 1:

    a = a * b;
    b = a / b;
    a = a / b;


Вариант 2:

    a = [b, b = a][0];


Второй вариант меня вообще поразил своей элегантностью :)

# Reto_-4_encuadernado_en_jupyter

Repositorio en donde se publica la evidencia de que mi persona, Lucas García, cumplió con el reto asignado.
***
[![Logo-equipo.webp](https://i.postimg.cc/Z5BYw1Tx/Logo-equipo.webp)](https://postimg.cc/9D2jMgwD)

# Inciso 1
Dado un número entero, determinar si ese número corresponde al código ASCII de una vocal minúscula.
```
num_ent: int

if __name__ == "__main__":
    num_ent = input("Digita un número para verificar si corresponde al código ASCII de una vocal minúscula")
    if num_ent == "97":
        print("Si corresponde y es el código de \"a\" ")
    elif num_ent == "101":
        print("Si corresponde y es el código de \"e\" ")
    elif num_ent == "105":
        print("Si corresponde y es el código de \"i\" ")
    elif num_ent == "111":
        print("Si corresponde y es el código de \"o\" ")
    elif num_ent == "117":
        print("Si corresponde y es el código de \"u\" ")
    else:
        print(num_ent, "No corresponde al código ASCII de ninguna vocal minúscula")
```

[![1.webp](https://i.postimg.cc/3xkXnzD1/1.webp)](https://postimg.cc/DSK4zj64)



# Inciso 2
Dada una cadena de longitud 1, determine si el código ASCII de primera letra de la cadena es par o no.
```
num : int

if __name__ == "__main__":
    cadena = str(input("Ingrese una cadena de longitud 1 (una letra, un símbolo, número, etc):"))
    if len(cadena) != 1:
        cadena = cadena[0]
        print("Ya que no ingresaste un solo carácter tomaré el primero, el cual es:", cadena)
    num = ord(cadena)
    print("El código ASCII del carácter (", cadena, ") es:", num)
    divisionSobreDos : int = int(num)%2
    if divisionSobreDos == 0: 
        print("y", str(num), "es par")
    else:
        print("y", str(num), "es impar")
```

[![2.webp](https://i.postimg.cc/6pFdSzrX/2.webp)](https://postimg.cc/rDC0R1Zn)



# Inciso 3
Dado un carácter, construya un programa en Python para determinar si el carácter es un dígito o no.
```
carac: str
x: bool = True

if __name__ == "__main__":

    while x == True:
        try:
            carac = int(input("Ingrese un carácter"))
            if carac >= 0 and carac <= 9:
                print(carac, "es un dígito")
            else:
                print(carac, "no es un dígito")
        except ValueError:
            print("Eso ni siquiera es un número")
        finally:
            break
```

[![3.webp](https://i.postimg.cc/ydH06dpp/3.webp)](https://postimg.cc/xk6Xt02L)



# Inciso 4
Dado un número real x, construya un programa que permita determinar si el número es positivo, negativo o cero. Para cada caso de debe imprimir el texto que se especifica a continuación:
- Positivo: "El número x es positivo"
- Negativo: "El número x es negativo"
- Cero (0): "El número x es el neutro para la suma"
```
real : float

if __name__ == "__main__":

    real = float(input("Ingresa un número"))
    if real > 0:
        print("El número", real, "es positivo")
    elif real < 0:
        print("El número", real, "es negativo")
    else:
        print("El número", real, "es neutro para la suma")
```

[![4.webp](https://i.postimg.cc/tgPhHPkV/4.webp)](https://postimg.cc/yJ1JmDwV)



# Inciso 5
Dado el centro y el radio de un círculo, determinar si un punto de R2 pertenece o no al interior del círculo.
```
centro_x: float
centro_y: float
radio_circulo : float
punt_x = float
punt_y = float

if __name__ == "__main__":

    print("Este programa te ayudará a verificar si un punto dentro de R2 se encuentra al interior del circulo")
    print("Por lo que ahora haz de ingresar los datos del círculo")
    centro_x = float(input("Coordenada en el eje x"))
    centro_y = float(input("Coordenada en el eje y"))
    radio_circulo = float(input("Radio"))

    print("Ahora ingresa las coordenadas del punto que desees")
    punt_x = float(input("En el eje x"))
    punt_y = float(input("En el eje y"))

    print("Y con estos datos tenemos que")

    if (punt_x-centro_x)**2 + (punt_y-centro_y)**2 < radio_circulo * radio_circulo:
        print("El punto (", punt_x, ",", punt_y, ") está dentro del círculo")
    elif (punt_x-centro_x)**2 + (punt_y-centro_y)**2 == radio_circulo * radio_circulo:
        print("El punto (", punt_x, ",", punt_y, ") está justo en la circunferencia")
    else:
        print("El punto (", punt_x, ",", punt_y, ") no está dentro del círculo")
```

[![5.webp](https://i.postimg.cc/G2xG4CZL/5.webp)](https://postimg.cc/34WdqP8V)



# Inciso 6
Dadas tres longitudes positivas, determinar si con esas longitudes se puede construir un triángulo.
```
a: float
b: float
c: float


if __name__ == "__main__":
    print("Ingresa 3 longitudes positivas y veremos si con ellas se puede construir un triángulo")
    a = float(input("La primera"))
    b = float(input("La segunda"))
    c = float(input("La tercera"))

    if a > 0 and b > 0 and c > 0:
        if a + b > c and c + a > b and b + c > a:
            print("Sí es posible formar un triángulo con estas medidas")
        else:
            print("No es posible formar un triángulo con estas medidas")
    elif a == 0 or b == 0 or c == 0:
        if a == 0:
            print(a, "es un valor inválido, intenta de nuevo")
        elif b == 0:
            print(b, "es un valor inválido, intenta de nuevo")
        else:
            print(c, "es un valor inválido, intenta de nuevo")
    else:
        print("Alguna(s) de tus longitudes es(son) negativa(s), intenta de nuevo con otros valores")
```

[![6.webp](https://i.postimg.cc/brYbb5hQ/6.webp)](https://postimg.cc/1nTf1J4t)


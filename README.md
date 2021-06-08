## Ejercicios Basicos de Python 

### Funciones Basicas (Bucle For I)

* imprime todos los enteros del 0 al 150.
```py
def printfrom0to150():
    for x in range(0, 151):
        print (x)
```

*  imprime todos los múltiplos de 5 de 5 a 1,000
```py
def ejercicio_2():
    for x in range(0, 1001):
        if x%5==0:
            print(x)

ejercicio_2()
```

* imprime enteros del 1 al 100. Si es divisible por 5, imprima "Coding" en su lugar. Si es divisible por 10, imprima "Coding Dojo".
```py
def ejercicio_3():
    for x in range(1, 101):
        if x%10==0:
            print("Coding Dojo")
        elif x%5==0:
            print("Coding")
        else:
            print(x)

ejercicio_3()
```

* suma enteros impares de 0 a 500,000 e imprime la suma final.
```py
def ejercicio_4():
    sum = 0
    for x in range(1, 500001):
        if x%2==1:
            sum = sum + x
    print(sum)
    return sum

ejercicio_4()
```

* imprime números positivos del 2018 al 0, restando 4 en cada iteración.
```py
def ejercicio_5():
    sum = 0
    for x in range(2018, 8, -4):
        sum = sum + x
    print(sum)
    return sum

ejercicio_5()
```

* establece tres variables: lowNum, highNum, mult. Comenzando en lowNum y pasando por highNum, imprima solo los enteros que son múltiplos de mult. Por ejemplo, si lowNum = 2, highNum = 9 y mult = 3, el bucle debe imprimir 3, 6, 9 (en líneas sucesivas)
```py
def ejercicio_6(lowNum, highNum, mult):
    for x in range(lowNum, highNum+1):
        if x%mult==0:
            print(x)

ejercicio_6(2, 9, 3)
```

* Probar con numeros primos
```py
def primos(num):
    for t in range(2,num):
        if num%t==0:
            return False
        return True

primos1000 = [x for x in range(2, 1001) if primos(x) is True]
```

### Funciones Basicas I

```py
#1
def a():
    return 5
print(a())

# 5
```

```py
#2
def a():
    return 5
print(a()+a())

# 10
```

```py
#3
def a():
    return 5
    return 10
print(a())
```

```py
#4
def a():
    return 5
    print(10)
print(a())

# 5
```

```py
#5
def a():
    print(5)
x = a()
print(x)

# 5
```

```py
#6
def a(b,c):
    print(b+c)
print(a(1,2) + a(2,3))

# 8
```

```py
#7
def a(b,c):
    return str(b)+str(c)
print(a(2,5))

# 25
```

```py
#8
def a():
    b = 100
    print(b)
    if b < 10:
        return 5
    else:
        return 10
    return 7
print(a())

# 100
# 10
```

```py
#9
def a(b,c):
    if b<c:
        return 7
    else:
        return 14
    return 3
print(a(2,3))
print(a(5,3))
print(a(2,3) + a(5,3))

# 7
# 14
# 21
```

```py
#10
def a(b,c):
    return b+c
    return 10
print(a(3,5))

# 8
```

```py
#11
b = 500
print(b)
def a():
    b = 300
    print(b)
print(b)
a()
print(b)

# 500
# 500
# 300
# 500
```

```py
#12
b = 500
print(b)
def a():
    b = 300
    print(b)
    return b
print(b)
a()
print(b)

# 500
# 500
# 300
# 300
# 500
```

```py
#13
b = 500
print(b)
def a():
    b = 300
    print(b)
    return b
print(b)
b=a()
print(b)

# 500
# 500
# 300
# 300
```

```py
#14
def a():
    print(1)
    b()
    print(2)
def b():
    print(3)
a()

# 1
# 3
# 2
```

```py
#15
def a():
    print(1)
    x = b()
    print(x)
    return 10
def b():
    print(3)
    return 5
y = a()
print(y)

# 1
# 3
# 5
# 10
```

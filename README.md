# Reto 10

Bienvenidos, espero esten bien, debo decir que este reto se me facilitó bastante así que espero no tenga errores y sea útil para el que lo vea.
Sin más que decir aquí están los ejercicios resueltos del reto 10

### 1 )  Desarrollar un algoritmo que calcule el promedio de un arreglo de reales.

```
# Desarrollar un algoritmo que calcule el promedio de un arreglo de reales.

lista = [] #creamos una lista vacía
real = float(input("ingrese los números reales para su arreglo: ")) #ingresamos el primer elemento de la lista
while (real != 999): #seguimos haciendo la pregunta hasta que el usuario ingrese '999'
    lista.append(real) #agregamos el elemento a la lista
    real = float(input("ingrese los números para su arreglo: (para terminar escriba '999')")) #volvemos a pedir elementos para la lista
print(lista) #imprimimos la lista

suma = sum(lista) # definimos 'suma' como la suma de los elementos de la lista
prom = suma / (len(lista)) # definimos 'prom' como la division entre la suma y la cantidad de elementos de la lista
print('el promedio de los números de su lista es ',prom) # imprimimos el promedio
```

### 2 ) Desarrollar un algoritmo que calcule el producto punto de dos arreglos de números enteros (reales) de igual tamaño.

```
lista1 = [] # creamos una lista 1 vacía
num = int(input("ingrese la cantidad de números que tendrá su arreglo: ")) # preguntamos cuantos elementos tendra la lista
for i in range(num): # pediremos los elementos la contidad de veces que el usuario dijo
    real = float(input("ingrese los números reales para su primer arreglo: ")) # pedimos los elementos de la lista
    lista1.append(real) # añadimos los elementos a la lista 1
print(lista1) #imprimimos la lista 1

lista2 = [] # creamos una lista 2 vacía
for j in range(num): # pediremos los elementos la contidad de veces que el usuario dijo
    real = float(input("ingrese los números reales para su segundo arreglo: ")) # pedimos los elementos de la lista
    lista2.append(real) # añadimos los elementos a la lista 2
print(lista2) #imprimimos la lista 2

lista3 = [] # creamos una lista 3 vacía
n = 0 #inicializamos n coomo '0'
for m in range(num):  # haremos el siguiente proceso por cada elemento de las listas
    mult = lista1[n]*lista2[n] # definimos 'mult' como la multiplicacion entre elementos de la misma posición de cada lista
    lista3.append(mult) # añadimos los resultados de las multiplicaciones en la lista 3
    n = n + 1 # sumamos '1' a 'n' para operar los elementos de la siguiente posicion
suma = sum(lista3) # definimos 'suma' como la suma de los elementos de la lista 3
print('el producto punto de los arreglos es ',suma) #imprimimos el producto punto
```
### 3 ) Hacer un algoritmo que deje al final de un arreglo de números todos los ceros que aparezcan en dicho arreglo.

```
# Hacer un algoritmo que deje al final de un arreglo de números todos los ceros que aparezcan en dicho arreglo.

lista1 = [] #creamos una lista vacía
num = int(input("ingrese la cantidad de números que tendrá su arreglo: ")) # preguntamos cuantos elementos tendra la lista
for i in range(num): # hacemos el siguiente proceso la cantidad de veces dicha por el usuario
    real = int(input("ingrese los números reales para su primer arreglo: ")) #pedimos los elementos de la lista
    lista1.append(real) # añadimos los elementos a la lista vacia
print(lista1) #imprimimos la lista

ceros = lista1.count(0) # definimoc 'ceros' como el conteo de '0' presentes en la lista
for j in range(ceros): # hacemos el siguiente proceso para cada '0' de la lista
    lista1.remove(0) # eliminamos los '0' de la lista

for m in range(ceros): # hacemos el siguiente proceso para cada '0' que habia en la lista
    lista1.append(0) #añadimos los '0' que habian al final de la lista

print('su lista con todos los ceros al final se ve asi: ',lista1) #imprimimos la lista
```

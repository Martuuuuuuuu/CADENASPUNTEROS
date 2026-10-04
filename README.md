# Actividad - Uso de punteros en la RAM

## Datos del proyecto

**Materia:** Laboratorio de Programación (LPR)
**Curso:** Año 5° División 3° 
**Institución:** E.E.S.T. N° 1 "Eduardo Ader"
**Profesor:** Prof. York
**Integrante:** Martina Araujo, Thiago Goya y Sofia Salaberry
**Archivo:** `main.cpp`

## Descripción

En este programa se trabaja con punteros para entender cómo se puede acceder a una variable mediante su dirección de memoria.

Se crea una variable llamada `edad` y un puntero llamado `p`:

```cpp
int edad = 0;
int* p = &edad;
```

El puntero `p` guarda la dirección de memoria de `edad`.

## Funcionamiento

El usuario ingresa su edad y el programa utiliza:

```cpp
cin >> *p;
```

El `*` permite acceder al valor que está guardado en la dirección a la que apunta `p`. Por eso, la edad ingresada se guarda directamente en la variable `edad`.

Después, el programa comprueba si la edad es mayor o igual a 18:

```cpp
if (*p >= 18)
```

Si se cumple, muestra que el acceso está aprobado. Si no, muestra que está rechazado.

También se muestra la dirección de memoria utilizando:

```cpp
cout << p;
```

En este caso se muestra la dirección de memoria y no el valor de la edad.

## Conceptos utilizados

* `&edad`: obtiene la dirección de memoria de `edad`.
* `p`: guarda esa dirección de memoria.
* `*p`: permite acceder al valor almacenado en esa dirección.
* `if`: permite comprobar si la edad es mayor o menor de 18.

## Ejemplo

Si el usuario ingresa:

```text
Ingrese su edad: 18
```

el programa muestra:

```text
[ACCESO APROBADO] El usuario es mayor de edad.
Edad registrada: 18 anos.
Direccion de memoria: 0x...
```

La dirección de memoria puede cambiar cada vez que se ejecuta el programa.

## Conclusión

Con esta actividad entendí que un puntero puede guardar la dirección de memoria de una variable y que, usando `*`, se puede acceder al valor que se encuentra en esa dirección.

También entendí la diferencia entre `p`, que muestra la dirección de memoria, y `*p`, que muestra o modifica el valor guardado en esa dirección.


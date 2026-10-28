# Ticket de salida 3

Nombre:Daniel Sanchez Sepulveda

Rol:202573043-K

Link al repositorio de GitHub (extra):

## Errores

### Error 1
- Tipo de error: acceso fuera de rango
- Línea del código:16
- Corrección: eliminacion en la parte del condicional del for el =

### Error 2
- Tipo de error:comienzo desde el segundo indice de mi arreglo que el primero y tambien de que en el for comenzamos a evaluar desde el tercer indice hasta el octabo(solo tenemos 7 indices en nuestro arr) por que lo perdemos contenido del indice inicial y tambien tenemos un acceso fuera de rango 
- Línea del código:24 y linea 25
- Corrección: incializar la variable dia en 0 y inicializar la variable del for en en 1 y la condicional que sea estrictamente menor que 7 para que no tengamos un acceso fuera de rango 

### Error 3
- Tipo de error:parte en el indice 1 en vez del 0 hasta llegar al septimo lo que daria un accseso fuera de rango
y que perderiamos el valor ingresado en la pos 0
- Línea del código:40
- Corrección: en el inicializador del for a la variable inicializarla en 0 y en la parte del condicional decirle que i debe ser menor estricto que 7 para que el for se repita solo 7 veces comenzando desde el 0

### Error 4
- Tipo de error:perdida de memoria, a la hora de liberar
- Línea del código:79
- Corrección: crear un for que libere la memoria fila por fila de la matriz dinamica que se creo, a la vez de liberar al final lo que quedo de la matriz dinamica para su completa eliminacion al final de nuestro codigo

### Error 5
- tipo de error: guardado mal tipo de dato ej si anotamos el dia 7 que seria el domingo estaria fuera de rango por lo que al guardar y que quede de 0 a 6 nuestro indices a la hora de guardar tenemos que guardarlo el numero del dia -1    
- linea de codigo: 53
-Correccion: a la hora de acceder a nuestro dia restarle 1 a la variable de indice que estamos recolectando con el scanf

## Caso de prueba propio (case_04)
```
6
0
3 90 6 10 6 100 6
0
3 10 3 20 4 90 4
0
4 90 4 200 6 100 6 50 1
```

```
Explicación: 
Ramo 1: 0                                                   = 0 minutos
Ramo 2: 90(domingo) + 10(domingo) + 100(domingo)            = 200 minutos
Ramo 3: 0                                                   = 0 minutos
Ramo 4: 10 (miercoles) + 20 (jueves) + 90 (jueves)          = 120 minutos
Ramo 5: 0                                                   = 0 minutos
Ramo 6: 90(jueves) +200(domingo) +100(domingo)+ 50(lunes)   = 440 minutos

El Domingo se entregan 90 + 10 + 100 + 100 + 200  = 500 minutos de tareas
```

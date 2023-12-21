Este es un home page del machetito legal que voy a usar en la evaluación jeje estoy re organizado

1. -Primero analizar todas las actividades de mas fácil a mas difícil 
2. -Hacer de las mas fácil a la mas difícil en una primera pasada donde haga lo principal y mas importante del programa (Ej.: El sistema que usa) 
3. -Volver a dar otra pasada de la mas fácil a la mas difícil pero esta vez donde agregue cosas menos necesarias (Ej.: "Escriba su numero el cual va a hacer esto y esto") 
4. -Repaso 
5. -Ultimos toques que me haya saltado

## DDF 1 
1.-  La calificación final de un estudiante de Informática y Programación se calcula con base a las calificaciones de cuatro aspectos de su rendimiento académico: participación, primer examen parcial, segundo examen parcial y examen final.  
Sabiendo que las calificaciones anteriores entran a la calificación final con ponderaciones del 10%, 25%, 25% y 40%, diseñar y codificar un algoritmo que calcule e imprima la calificación final obtenida por un estudiante.

Algoritmo CalificacionFinal
    Escribir "Ingrese la participación del alumno: "
    Leer participacion
    Escribir "Ingrese la calificación del primer examen parcial: "
    Leer examenParcial1
    Escribir "Ingrese la calificación del segundo examen parcial: "
    Leer examenParcial2
    Escribir "Ingrese la calificación del examen final: "
    Leer examenFinal

    calificacionFinal <- (participacion * 0.1) + (examenParcial1 * 0.25) + (examenParcial2 * 0.25) + (examenFinal * 0.4)

    Escribir "La calificación final es: ", calificacionFinal
FinAlgoritmo


---


2.-  La fábrica de sillas “El Reposo Feliz” paga a sus obreros la cantidad de $50 por cada silla que fabrica por día. No obstante, si el número de sillas fabricadas por un obrero supera las cinco diarias, el pago es de $60 por cada una, más un 2% del total de las ventas diarias realizadas.  
En el día se logran vender todas las sillas fabricadas a un valor de $130 cada una.  
Diseñar y codificar un algoritmo que lea las cantidades correspondientes y que calcule e imprima el salario diario de un empleado.  

Algoritmo SalarioDiario
    Escribir "Ingrese la cantidad de sillas fabricadas por el obrero: "
    Leer sillasFabricadas

    Si sillasFabricadas <= 5 Hacer
        salario <- sillasFabricadas * 50
    Sino
        salario <- (sillasFabricadas * 60) + (0.02 * sillasFabricadas * 130)
    FinSi

    Escribir "El salario diario del empleado es: ", salario
FinAlgoritmo


---


3.-  Diseñar un algoritmo que calcule e imprima la diferencia entre dos números enteros ingresados por teclado restando siempre del más grande el más chico.  

Algoritmo DiferenciaEntreNumeros
    Escribir "Ingrese el primer número: "
    Leer num1
    Escribir "Ingrese el segundo número: "
    Leer num2

    Si num1 > num2 Hacer
        diferencia <- num1 - num2
    Sino
        diferencia <- num2 - num1
    FinSi

    Escribir "La diferencia entre los números es: ", diferencia
FinAlgoritmo


---


4.-  Diseñar y codificar un algoritmo que lea dos números enteros y que determine y muestre la suma entre ellos si son de igual signo.  

Algoritmo SumaIgualSigno
    Escribir "Ingrese el primer número entero: "
    Leer num1
    Escribir "Ingrese el segundo número entero: "
    Leer num2

    Si (num1 > 0 y num2 > 0) o (num1 < 0 y num2 < 0) Hacer
        suma <- num1 + num2
        Escribir "La suma de los números es: ", suma
    Sino
        Escribir "Los números no tienen el mismo signo."
    FinSi
FinAlgoritmo


---


5.- La compañía ABC aplica dos pruebas a cada persona que desea ingresar a la misma. Se la contrata si obtiene un mínimo de 75 puntos en cada de ellas, en caso contrario se le rechaza.  
Diseñar y codificar un algoritmo que lea las cantidades pertinentes y que determine si una persona es aceptada por la compañía ABC.  

Algoritmo AceptacionEnCompaniaABC
    Escribir "Ingrese la calificación de la primera prueba: "
    Leer prueba1
    Escribir "Ingrese la calificación de la segunda prueba: "
    Leer prueba2

    Si prueba1 >= 75 y prueba2 >= 75 Hacer
        Escribir "La persona es aceptada en la compañía ABC."
    Sino
        Escribir "La persona es rechazada en la compañía ABC."
    FinSi
FinAlgoritmo


---

6.-  Hacer un programa que solicite el ingreso de tres números por teclado y calcule y muestre la suma de los dos mayores.  

Algoritmo SumaDosMayores
    Escribir "Ingrese el primer número: "
    Leer num1
    Escribir "Ingrese el segundo número: "
    Leer num2
    Escribir "Ingrese el tercer número: "
    Leer num3

    // Ordenar los números de mayor a menor
    Si num1 < num2 Hacer
        intercambiar(num1, num2)
    FinSi
    Si num2 < num3 Hacer
        intercambiar(num2, num3)
    FinSi
    Si num1 < num2 Hacer
        intercambiar(num1, num2)
    FinSi

    sumaDosMayores <- num1 + num2
    Escribir "La suma de los dos mayores números es: ", sumaDosMayores
FinAlgoritmo


---


7.-  Diseñar y codificar un algoritmo que lea tres números enteros y que calcule e imprima la diferencia entre los dos mayores y el producto de los dos más chicos.  

Algoritmo DiferenciaYProducto
    Escribir "Ingrese el primer número entero: "
    Leer num1
    Escribir "Ingrese el segundo número entero: "
    Leer num2
    Escribir "Ingrese el tercer número entero: "
    Leer num3

    // Ordenar los números de mayor a menor
    Si num1 < num2 Hacer
        intercambiar(num1, num2)
    FinSi
    Si num2 < num3 Hacer
        intercambiar(num2, num3)
    FinSi
    Si num1 < num2 Hacer
        intercambiar(num1, num2)
    FinSi

    diferenciaDosMayores <- num1 - num2
    productoDosMenores <- num2 * num3

    Escribir "La diferencia entre los dos mayores números es: ", diferenciaDosMayores
    Escribir "El producto de los dos menores números es: ", productoDosMenores
FinAlgoritmo


---


8.-  Diseñar un algoritmo que lea los valores de x y de d, y que imprima el valor final de d, calculado de acuerdo a las siguientes expresiones:  
si x <= 1,     si d > 100,        sumar a    d      un 20 %  
si 1 < x <= 2,        si d > 100,        sumar a    d      un 30 %  
si 2 < x <= 3,        si d > 100,        sumar a    d      un 40 %  
si x > 3, si d > 100,    sumar a    d      un 50 %  

Algoritmo CalculoValorFinalD
    Escribir "Ingrese el valor de x: "
    Leer x
    Escribir "Ingrese el valor de d: "
    Leer d

    Si x <= 1 y d > 100 Hacer
        d <- d + (0.2 * d)
    Sino Si x > 1 y x <= 2 y d > 100 Hacer
        d <- d + (0.3 * d)
    Sino Si x > 2 y x <= 3 y d > 100 Hacer
        d <- d + (0.4 * d)
    Sino Si x > 3 y d > 100 Hacer
        d <- d + (0.5 * d)
    FinSi

    Escribir "El valor final de d es: ", d
FinAlgoritmo


---

9.-  Una Oficina de Correos aplica la siguiente la siguiente tarifa para sus envíos como cartas:  
$ 10.00           por los primeros 20 gramos.  
$  2.00          por gramo, para los siguientes 10 gramos. 
$  1.50         por gramo, hasta 200 gramos.  
Si la carta supera los 200 gramos, no es aceptada como tal.  
Diseñar un algoritmo que lea el peso de un envío y que determine, si corresponde, el pago que se debe hacer.

Algoritmo TarifaEnviosCartas
    Escribir "Ingrese el peso del envío en gramos: "
    Leer peso

    Si peso <= 20 Hacer
        tarifa <- 10
    Sino Si peso <= 30 Hacer
        tarifa <- 10 + 2 * (peso - 20)
    Sino Si peso <= 200 Hacer
        tarifa <- 10 + 2 * 10 + 1.5 * (peso - 30)
    Sino
        Escribir "El envío no es aceptado, ya que supera los 200 gramos."
        Terminar
    FinSi

    Escribir "La tarifa para el envío es: ", tarifa
FinAlgoritmo



## DDF 2 
1) Convertir en segundos, una hora que viene expresada en horas, minutos y segundos. Ingresar los datos y visualizar por pantallas los segundos totales.  

Algoritmo ConvertirAHorasMinutosSegundos
    Escribir "Ingrese la cantidad de horas: "
    Leer horas
    Escribir "Ingrese la cantidad de minutos: "
    Leer minutos
    Escribir "Ingrese la cantidad de segundos: "
    Leer segundos

    totalSegundos <- segundos + (minutos * 60) + (horas * 3600)

    Escribir "El tiempo total en segundos es: ", totalSegundos
FinAlgoritmo



---

2) Convertir a horas, minutos y segundos, un tiempo que viene expresadao en segundos. Ingresar los datos y visualizar por pantallas los valores obtenidos en formato hh:mm:ss.  

Algoritmo ConvertirASegundos
    Escribir "Ingrese la cantidad de segundos: "
    Leer totalSegundos

    horas <- totalSegundos / 3600
    minutos <- (totalSegundos % 3600) / 60
    segundos <- totalSegundos % 60

    Escribir "El tiempo en formato hh:mm:ss es: ", horas, ":", minutos, ":", segundos
FinAlgoritmo



---

3) Dados 3 lados de un triángulo, informar si el mismo es equilátero, isósceles o escaleno.  

Algoritmo TipoTriangulo
    Escribir "Ingrese el lado 1 del triángulo: "
    Leer lado1
    Escribir "Ingrese el lado 2 del triángulo: "
    Leer lado2
    Escribir "Ingrese el lado 3 del triángulo: "
    Leer lado3

    Si lado1 = lado2 y lado2 = lado3 Hacer
        Escribir "El triángulo es equilátero."
    Sino Si lado1 = lado2 o lado2 = lado3 o lado1 = lado3 Hacer
        Escribir "El triángulo es isósceles."
    Sino
        Escribir "El triángulo es escaleno."
    FinSi
FinAlgoritmo


---

4) Diseñar un algoritmo que calcule e imprima la cantidad de dinero que corresponde a cada uno de los tres socios de una empresa conociendo la cantidad de dinero a distribuir y sabiendo que el segundo y el tercero recibirán la mitad de lo que le corresponde al primero.  


Algoritmo DistribucionDineroSocios
    Escribir "Ingrese la cantidad de dinero a distribuir: "
    Leer dineroTotal

    dineroPrimerSocio <- dineroTotal / 2
    dineroSegundoSocio <- dineroPrimerSocio / 2
    dineroTercerSocio <- dineroSegundoSocio

    Escribir "Dinero para el primer socio: ", dineroPrimerSocio
    Escribir "Dinero para el segundo socio: ", dineroSegundoSocio
    Escribir "Dinero para el tercer socio: ", dineroTercerSocio
FinAlgoritmo



---

5) Diseñar un algoritmo que calcule y muestre el salario mensual de un empleado a partir de sus horas trabajadas y del valor hora establecido. La cantidad de horas trabajadas que superen las 160 se pagan a un valor de un 50% adicional. En cambio, las que superen las 200 se abonan al doble de su valor hora original. Al salario mensual calculado se le debe descontar un 5% en concepto de aportes y contribuciones siempre que su sueldo bruto no supere los $5000.  

Algoritmo SalarioMensual
    Escribir "Ingrese la cantidad de horas trabajadas: "
    Leer horasTrabajadas
    Escribir "Ingrese el valor por hora establecido: "
    Leer valorHora

    Si horasTrabajadas > 200 Hacer
        salario <- 200 * valorHora + 2 * (horasTrabajadas - 200) * valorHora
    Sino Si horasTrabajadas > 160 Hacer
        salario <- horasTrabajadas * valorHora + 0.5 * (horasTrabajadas - 160) * valorHora
    Sino
        salario <- horasTrabajadas * valorHora
    FinSi

    // Aplicar descuentos si el salario bruto no supera $5000
    Si salario <= 5000 Hacer
        salario <- salario - 0.05 * salario
    FinSi

    Escribir "El salario mensual calculado es: ", salario
FinAlgoritmo


---

6) Diseñar y codificar un algoritmo que lea dos números enteros y que determine y muestre la suma entre ellos si son de igual signo.




## DDF 3
1.- Hacer un diagrama de flujo (DDF) que pida dos números enteros. El programa pedirá de nuevo el segundo número mientras no sea mayor que el primero. El programa terminará escribiendo los dos números.  

---

2.- Hacer un DDF que muestre los primeros 30 naturales.  


Algoritmo BucleSegundoMayor
    Escribir "Ingrese el primer número: "
    Leer num1
    Escribir "Ingrese el segundo número (debe ser mayor al primero): "
    Leer num2

    Mientras num2 <= num1 Hacer
        Escribir "El segundo número debe ser mayor al primero. Inténtelo de nuevo



---

3.- Escriba un DDF que pida números entero mientras el usuario escriba número mayores que el primero.  

Algoritmo BucleNumerosMayores
    Escribir "Ingrese el primer número: "
    Leer num1
    Escribir "Ingrese un número (ingrese un número menor o igual al primero para detenerse): "
    Leer num

    Mientras num <= num1 Hacer
        Escribir "Ingrese un número mayor al primero para continuar o igualarlo para detenerse: "
        Leer num
    FinMientras
FinAlgoritmo



---

4.- Diseñar un DDF que calcule y muestre el promedio de 10 números.  

Algoritmo PromedioDiezNumeros
    suma <- 0

    Desde i <- 1 Hasta 10 Con Paso 1 Hacer
        Escribir "Ingrese el número ", i, ": "
        Leer num
        suma <- suma + num
    FinDesde

    promedio <- suma / 10

    Escribir "El promedio de los 10 números es: ", promedio
FinAlgoritmo



---

5.- Realizar un DDF que permita el ingreso de 10 números y calcule el mayor y el menor. Los números son todos positivos.  

Algoritmo MayorMenorDiezNumeros
    mayor <- 0
    menor <- 0

    Desde i <- 1 Hasta 10 Con Paso 1 Hacer
        Escribir "Ingrese el número ", i, ": "
        Leer num

        Si i = 1 Hacer
            mayor <- num
            menor <- num
        Sino
            Si num > mayor Hacer
                mayor <- num
            FinSi
            Si num < menor Hacer
                menor <- num
            FinSi
        FinSi
    FinDesde

    Escribir "El número mayor es: ", mayor
    Escribir "El número menor es: ", menor
FinAlgoritmo



---

6.- Escriba un DDF que pida números enteros mientras sean cada vez más grandes.  

Algoritmo BucleNumerosCadaVezMasGrandes
    Escribir "Ingrese el primer número: "
    Leer num1
    Escribir "Ingrese un número mayor al primero: "
    Leer num

    Mientras num > num1 Hacer
        num1 <- num
        Escribir "Ingrese un número mayor al último ingresado: "
        Leer num
    FinMientras
FinAlgoritmo



---

7.- Desarrollar un DDF que permita calcular el área de un triángulo conociendo la base y la altura. Tiene que validar que los valores de los datos tengan sentido.  

Algoritmo AreaTriangulo
    Escribir "Ingrese la base del triángulo: "
    Leer base
    Escribir "Ingrese la altura del triángulo: "
    Leer altura

    // Validar que los valores tengan sentido
    Si base <= 0 o altura <= 0 Hacer
        Escribir "Los valores de base y altura deben ser positivos."
        Terminar
    FinSi

    area <- (base * altura) / 2

    Escribir "El área del triángulo es: ", area
FinAlgoritmo


---

8.- Escriba un DDF que pida la cantidad de números positivos que se tienen que escribir y a continuación pida números hasta que se haya escrito la cantidad de números positivos indicada.

Algoritmo IngresoCantidadNumerosPositivos
    Escribir "Ingrese la cantidad de números positivos que desea escribir: "
    Leer cantidadNumeros

    Desde i <- 1 Hasta cantidadNumeros Con Paso 1 Hacer
        Escribir "Ingrese el número ", i, ": "
        Leer num
        // Puedes realizar operaciones con 'num' aquí si lo necesitas
    FinDesde
FinAlgoritmo

## DDF 4 
1) Desarrollar un programa que muestre el listado de números enteros que hay entre otros dos que se ingresan por teclado.  

Algoritmo ListadoNumerosEntreDos
    Escribir "Ingrese el primer número: "
    Leer num1
    Escribir "Ingrese el segundo número: "
    Leer num2

    Desde i <- num1 + 1 Hasta num2 - 1 Con Paso 1 Hacer
        Escribir i
    FinDesde
FinAlgoritmo


---

2) Diseñar un algoritmo que lea los salarios de los N trabajadores de una empresa y que determine cuántos de ellos ganan más de $ 2.500. El valor de N se debe solicitar al inicio del algoritmo.  

Algoritmo SalariosMayores2500
    Escribir "Ingrese la cantidad de trabajadores: "
    Leer cantidadTrabajadores
    contadorSalariosMayores2500 <- 0

    Desde i <- 1 Hasta cantidadTrabajadores Con Paso 1 Hacer
        Escribir "Ingrese el salario del trabajador ", i, ": "
        Leer salario

        Si salario > 2500 Hacer
            contadorSalariosMayores2500 <- contadorSalariosMayores2500 + 1
        FinSi
    FinDesde

    Escribir "La cantidad de trabajadores con salario mayor a $2500 es: ", contadorSalariosMayores2500
FinAlgoritmo


---

3) Hacer un algoritmo que pida que se ingrese la edad de un grupo de estudiantes y, al finalizar, muestre la edad del más viejo y la cantidad que hay con esa edad (la del más viejo). El ingreso de datos debe finalizar cuando se ingrese un cero

Algoritmo EstudianteMasViejo
    edadMasVieja <- 0
    cantidadEstudiantesMasViejos <- 0

    Escribir "Ingrese la edad del estudiante (ingrese 0 para terminar): "
    Leer edad

    Mientras edad <> 0 Hacer
        Si edad > edadMasVieja Hacer
            edadMasVieja <- edad
            cantidadEstudiantesMasViejos <- 1
        Sino Si edad = edadMasVieja Hacer
            cantidadEstudiantesMasViejos <- cantidadEstudiantesMasViejos + 1
        FinSi

        Escribir "Ingrese la edad del siguiente estudiante (ingrese 0 para terminar): "
        Leer edad
    FinMientras

    Escribir "La edad del estudiante más viejo es: ", edadMasVieja
    Escribir "La cantidad de estudiantes con esa edad es: ", cantidadEstudiantesMasViejos
FinAlgoritmo


## DDF 5 
1.- Diseñar un algoritmo que reciba como entrada la temperatura al medio día de cada uno de los días de una semana determinada. El programa deberá encontrar la temperatura promedio al medio día, pero sólo para aquellos días en que la misma fuera superior a los 10ºC.  

Algoritmo TemperaturaPromedio
    sumaTemperaturas <- 0
    cantidadDias <- 0

    Para cada día de la semana Hacer
        Escribir "Ingrese la temperatura al mediodía del ", día
        Leer temperatura

        Si temperatura > 10 Hacer
            sumaTemperaturas <- sumaTemperaturas + temperatura
            cantidadDias <- cantidadDias + 1
        FinSi
    FinPara

    Si cantidadDias > 0 Hacer
        temperaturaPromedio <- sumaTemperaturas / cantidadDias
        Escribir "La temperatura promedio al mediodía es: ", temperaturaPromedio
    Sino
        Escribir "No se ingresaron temperaturas superiores a 10°C."
    FinSi
FinAl


---
  
2.- Desarrollar un algoritmo que lea las calificaciones obtenidas en Matemática por los alumnos de un salón; este algoritmo deberá calcular e imprimir el promedio obtenido por el salón y el promedio de los que aprobaron la materia. El número de alumnos es conocido.  

Algoritmo PromedioCalificacionesMatematicas
    sumaCalificaciones <- 0
    cantidadAlumnos <- 0

    Escribir "Ingrese la cantidad de alumnos en el salón: "
    Leer cantidadAlumnos

    Para cada alumno desde 1 hasta cantidadAlumnos Hacer
        Escribir "Ingrese la calificación en Matemáticas del alumno ", alumno
        Leer calificacion

        sumaCalificaciones <- sumaCalificaciones + calificacion
    FinPara

    promedioTotal <- sumaCalificaciones / cantidadAlumnos

    Escribir "El promedio general en Matemáticas es: ", promedioTotal
FinAlgoritmo


---

3.- Escriba un programa que pida números pares mientras el usuario indique que quiere seguir introduciendo números. Para indicar que quiere seguir escribiendo números, el usuario deberá contestar S o s a la pregunta

Algoritmo PromedioCalificacionesMatematicas
    sumaCalificaciones <- 0
    cantidadAlumnos <- 0

    Escribir "Ingrese la cantidad de alumnos en el salón: "
    Leer cantidadAlumnos

    Para cada alumno desde 1 hasta cantidadAlumnos Hacer
        Escribir "Ingrese la calificación en Matemáticas del alumno ", alumno
        Leer calificacion

        sumaCalificaciones <- sumaCalificaciones + calificacion
    FinPara

    promedioTotal <- sumaCalificaciones / cantidadAlumnos

    Escribir "El promedio general en Matemáticas es: ", promedioTotal
FinAlgoritmo


# MARDITO MACHETE LEGAL RRR

### Temas de Programación: DDF 1

#### 1. Cálculos con Ponderaciones:

##### Actividad 1 - Calificación Final de un Estudiante:
**Descripción:**
La calificación final de un estudiante se calcula con base en cuatro aspectos de su rendimiento académico, cada uno con una ponderación específica.

**Pasos:**
1. **Entrada de Datos:**
   - Solicita al usuario ingresar las calificaciones de participación, primer examen parcial, segundo examen parcial y examen final.
   ```pseudocode
   Leer participacion
   Leer parcial1
   Leer parcial2
   Leer final
   ```

2. **Cálculo de Ponderaciones:**
   - Aplica las ponderaciones a las calificaciones ingresadas.
   ```pseudocode
   ponderacion_participacion = participacion * 0.10
   ponderacion_parcial1 = parcial1 * 0.25
   ponderacion_parcial2 = parcial2 * 0.25
   ponderacion_final = final * 0.40
   ```

3. **Cálculo de Calificación Final:**
   - Suma las calificaciones ponderadas para obtener la calificación final.
   ```pseudocode
   calificacion_final = ponderacion_participacion + ponderacion_parcial1 + ponderacion_parcial2 + ponderacion_final
   ```

4. **Impresión de Resultados:**
   - Muestra la calificación final obtenida por el estudiante.
   ```pseudocode
   Imprimir "Calificación Final: ", calificacion_final
   ```

##### Actividad 2 - Salario Diario de un Empleado:
**Descripción:**
Calcula el salario diario de un empleado basado en la cantidad de sillas fabricadas y vendidas.

**Pasos:**
1. **Entrada de Datos:**
   - Solicita al usuario ingresar la cantidad de sillas fabricadas por el empleado.
   ```pseudocode
   Leer sillas_fabricadas
   ```

2. **Cálculo de Salario:**
   - Aplica las condiciones para calcular el salario diario.
   ```pseudocode
   si sillas_fabricadas <= 5 entonces
       salario = sillas_fabricadas * 50
   sino
       salario = (sillas_fabricadas * 60) + (0.02 * (sillas_fabricadas * 130))
   fin_si
   ```

3. **Impresión de Resultados:**
   - Muestra el salario diario del empleado.
   ```pseudocode
   Imprimir "Salario Diario: $", salario
   ```

#### 2. Operaciones Básicas y Estructuras Condicionales:

##### Actividad 3 - Diferencia entre Dos Números:
**Descripción:**
Calcula e imprime la diferencia entre dos números enteros.

**Pasos:**
1. **Entrada de Datos:**
   - Solicita al usuario ingresar dos números enteros.
   ```pseudocode
   Leer numero1
   Leer numero2
   ```

2. **Cálculo de Diferencia:**
   - Determina el número más grande y resta el más chico.
   ```pseudocode
   si numero1 > numero2 entonces
       diferencia = numero1 - numero2
   sino
       diferencia = numero2 - numero1
   fin_si
   ```

3. **Impresión de Resultados:**
   - Muestra la diferencia entre los dos números.
   ```pseudocode
   Imprimir "Diferencia: ", diferencia
   ```

##### Actividad 4 - Suma de Números de Igual Signo:
**Descripción:**
Lee dos números enteros y muestra la suma solo si ambos tienen el mismo signo.

**Pasos:**
1. **Entrada de Datos:**
   - Solicita al usuario ingresar dos números enteros.
   ```pseudocode
   Leer num1
   Leer num2
   ```

2. **Verificación de Signos:**
   - Determina si ambos números tienen el mismo signo.
   ```pseudocode
   si (num1 > 0 y num2 > 0) o (num1 < 0 y num2 < 0) entonces
       suma = num1 + num2
       Imprimir "Suma: ", suma
   sino
       Imprimir "Los números no tienen el mismo signo."
   fin_si
   ```

### Temas de Programación: DDF 2

#### 1. Conversión y Manipulación de Tiempo:

##### Actividad 1 - Conversión de Tiempo:
**Descripción:**
Convierte una hora de formato horas:minutos:segundos a segundos.

**Pasos:**
1. **Entrada de Datos:**
   - Solicita al usuario ingresar las horas, minutos y segundos.
   ```pseudocode
   Leer horas
   Leer minutos
   Leer segundos
   ```

2. **Cálculo de Segundos:**
   - Convierte la hora a segundos.
   ```pseudocode
   total_segundos = (horas * 3600) + (minutos * 60) + segundos
   ```

3. **Impresión de Resultados:**
   - Muestra los segundos totales.
   ```pseudocode
   Imprimir "Segundos totales: ", total_segundos
   ```

##### Actividad 2 - Conversión a Tiempo:
**Descripción:**
Convierte un tiempo dado en segundos a formato horas:minutos:segundos.

**Pasos:**
1. **Entrada de Datos:**
   - Solicita al usuario ingresar los segundos.
   ```pseudocode
   Leer total_segundos
   ```

2. **Cálculo de Tiempo:**
   - Convierte los segundos a formato horas:minutos:segundos.
   ```pseudocode
   horas = total_segundos / 3600
   minutos = (total_segundos % 3600) / 60
   segundos = total_segundos % 60
   ```

3. **Impresión de Resultados:**
   - Muestra el tiempo en formato hh:mm:ss.
   ```pseudocode
   Imprimir "Tiempo: ", horas, " horas, ", minutos, " minutos, ", segundos, " segundos"
   ```

##### Actividad 3 - Clasificación de Triángulos:
**Descripción:**
Dados tres lados de un triángulo, determina si es equilátero, isósceles o escaleno.

**Pasos:**
1. **Entrada de Datos:**
   - Solicita al usuario ingresar los tres lados del triángulo.
   ```pseudocode
   Leer lado1
   Leer lado2
   Leer lado3
   ```

2. **Verificación de Clasificación:**
   - Verifica si el triángulo es equilátero, isósceles o escaleno.
   ```pseudocode
   si lado1 = lado2 y lado2 = lado3 entonces
       Imprimir "Triángulo Equilátero"
   sino si lado1 = lado2 o lado1 = lado3 o lado2 = lado3 entonces
       Imprimir "Triángulo Isósceles"
   sino
       Imprimir "Triángulo Escaleno"
   fin_si
   ```

#### 2. Operaciones Matemáticas y Distribución de Dinero:

##### Actividad 4 - Distribución de Dinero entre Socios:
**Descripción:**
Calcula la cantidad de dinero que corresponde a cada uno de los tres socios de una empresa.

**Pasos:**
1. **Entrada de Datos:**
   - Solicita al usuario ingresar la cantidad de dinero a distribuir.
   ```pseudocode
   Leer dinero_a_distribuir
   ```

2. **Cálculo de Distribución:**
   - Calcula la cantidad de dinero que recibe cada socio.
   ```pseudocode
   primer_socio = dinero_a_distribuir / 2
   segundo_socio = dinero_a_distribuir / 4
   tercer_socio = dinero_a_distribuir / 4
   ```

3. **Impresión de Resultados:**
   - Muestra la cantidad de dinero que recibe cada socio.
   ```pseudocode
   Imprimir "Primer Socio: $", primer_socio
   Imprimir "Segundo Socio: $", segundo_socio
   Imprimir "Tercer Socio: $", tercer_socio
   ```

##### Actividad 5 - Cálculo de Salario Mensual:
**Descripción:**
Calcula el salario mensual de un empleado considerando horas trabajadas y tarifas específicas.

**Pasos:**
1. **Entrada de Datos:**
   - Solicita al usuario ingresar las horas trabajadas y el valor hora.
   ```pseudocode
   Leer horas_trabajadas
   Leer valor_hora
   ```

2. **Cálculo de Salario:**
   - Calcula el salario considerando horas extras y descuentos.
   ```pseudocode
   si horas_trabajadas > 160 entonces
       salario = (160 * valor_hora) + ((horas_trabajadas - 160) * valor_hora * 1.5)
   sino
       salario = horas_trabajadas * valor_hora
   fin_si

   si salario > 5000 entonces
       descuento = 0.05 * salario
       salario = salario - descuento
   fin_si
   ```

3. **Impresión de Resultados:**
   - Muestra el salario mensual del empleado.
   ```pseudocode
   Imprimir "Salario Mensual: $", salario
   ```

### Temas de Programación: DDF 3

#### 1. Control de Flujo y Bucles:

##### Actividad 1 - Bucle hasta que se Cumpla una Condición:
**Descripción:**
Pide dos números enteros. El programa solicitará el segundo número nuevamente mientras no sea mayor que el primero. El programa terminará escribiendo los dos números.

**Pasos:**
1. **Bucle para Ingresar Números:**
   - Utiliza un bucle para asegurarse de que el segundo número sea mayor que el primero.
   ```pseudocode
   Leer num1
   Leer num2

   mientras num2 <= num1 hacer
       Imprimir "El segundo número debe ser mayor que el primero. Inténtalo de nuevo."
       Leer num2
   fin_mientras

   Imprimir "Los números ingresados son: ", num1, " y ", num2
   ```

##### Actividad 2 - Mostrar los Primeros 30 Naturales:
**Descripción:**
Muestra los primeros 30 números naturales.

**Pasos:**
1. **Bucle para Mostrar Números:**
   - Utiliza un bucle para mostrar los primeros 30 números naturales.
   ```pseudocode
   desde i = 1 hasta 30 hacer
       Imprimir i
   fin_desde
   ```

##### Actividad 3 - Bucle mientras se Ingresan Números Mayores:
**Descripción:**
Pide números enteros mientras el usuario escriba números mayores que el primero.

**Pasos:**
1. **Bucle para Ingresar Números:**
   - Utiliza un bucle para solicitar números mientras sean mayores que el primero.
   ```pseudocode
   Leer num1
   Leer num

   mientras num > num1 hacer
       Imprimir "Ingresa otro número (o un número menor que el primero para salir): "
       Leer num
   fin_mientras
   ```

##### Actividad 4 - Cálculo y Muestra del Promedio:
**Descripción:**
Calcula y muestra el promedio de 10 números.

**Pasos:**
1. **Bucle para Ingresar Números:**
   - Utiliza un bucle para ingresar 10 números y calcular la suma.
   ```pseudocode
   suma = 0
   desde i = 1 hasta 10 hacer
       Imprimir "Ingresa el número ", i, ": "
       Leer num
       suma = suma + num
   fin_desde

   promedio = suma / 10
   Imprimir "El promedio es: ", promedio
   ```

##### Actividad 5 - Encontrar el Mayor y Menor:
**Descripción:**
Lee 10 números positivos y calcula el mayor y el menor.

**Pasos:**
1. **Bucle para Ingresar Números:**
   - Utiliza un bucle para ingresar 10 números y encontrar el mayor y el menor.
   ```pseudocode
   mayor = 0
   menor = infinito

   desde i = 1 hasta 10 hacer
       Imprimir "Ingresa el número ", i, ": "
       Leer num

       si num > mayor entonces
           mayor = num
       fin_si

       si num < menor entonces
           menor = num
       fin_si
   fin_desde

   Imprimir "El número mayor es: ", mayor
   Imprimir "El número menor es: ", menor
   ```

##### Actividad 6 - Bucle hasta que se Ingresen Números cada vez Mayores:
**Descripción:**
Pide números enteros mientras sean cada vez mayores.

**Pasos:**
1. **Bucle para Ingresar Números:**
   - Utiliza un bucle para solicitar números mientras cada número ingresado sea mayor que el anterior.
   ```pseudocode
   Imprimir "Ingresa el primer número: "
   Leer num_anterior

   mientras verdadero hacer
       Imprimir "Ingresa otro número (o un número menor para salir): "
       Leer num

       si num <= num_anterior entonces
           Imprimir "Fin del programa."
           romper  // Sale del bucle
       fin_si

       num_anterior = num
   fin_mientras
   ```

##### Actividad 7 - Cálculo de Área de Triángulo con Validación:
**Descripción:**
Calcula el área de un triángulo conociendo la base y la altura, validando que los valores tengan sentido.

**Pasos:**
1. **Entrada de Datos con Validación:**
   - Utiliza un bucle para solicitar la base y la altura asegurándose de que ambos sean mayores que cero.
   ```pseudocode
   Leer base
   Leer altura

   mientras base <= 0 o altura <= 0 hacer
       Imprimir "La base y la altura deben ser mayores que cero. Inténtalo de nuevo."
       Leer base
       Leer altura
   fin_mientras
   ```

2. **Cálculo de Área:**
   - Calcula el área del triángulo.
   ```pseudocode
   area = (base * altura) / 2
   ```

3. **Impresión de Resultados:**
   - Muestra el área del triángulo.
   ```pseudocode
   Imprimir "Área del triángulo: ", area
   ```

##### Actividad 8 - Ingreso de Números Positivos según Cantidad Indicada:
**Descripción:**
Pide la cantidad de números positivos que se deben escribir y solicita esos números al usuario.

**Pasos:**
1. **Entrada de Datos:**
   - Solicita al usuario la cantidad de números positivos que se deben ingresar.
   ```pseudocode
   Leer cantidad_a_ingresar
   ```

2. **Bucle para Ingresar Números:**
   - Utiliza un bucle para solicitar la cantidad específica de números positivos.
   ```pseudocode
   desde i = 1 hasta cantidad_a_ingresar hacer
       Imprimir "Ingresa el número positivo ", i, ": "
       Leer num
       mientras num <= 0 hacer
           Imprimir "Debes ingresar un número positivo. Inténtalo de nuevo."
           Leer num
       fin_mientras
   fin_desde
   ```

### Temas de Programación: DDF 4

#### 1. Estructuras de Control y Manejo de Listas:

##### Actividad 1 - Mostrar Números entre Dos Ingresados:
**Descripción:**
Muestra el listado de números enteros que hay entre dos números ingresados por teclado.

**Pasos:**
1. **Entrada de Datos:**
   - Solicita al usuario ingresar los dos números entre los cuales se mostrarán los enteros.
   ```pseudocode
   Leer num1
   Leer num2
   ```

2. **Mostrar Números entre Dos Ingresados:**
   - Utiliza un bucle para mostrar los números enteros entre los dos ingresados.
   ```pseudocode
   desde i = num1 hasta num2 hacer
       Imprimir i
   fin_desde
   ```

##### Actividad 2 - Cálculo de Trabajadores que Ganan más de $2,500:
**Descripción:**
Lee los salarios de los N trabajadores de una empresa y determina cuántos ganan más de $2,500.

**Pasos:**
1. **Entrada de Datos:**
   - Solicita al usuario ingresar la cantidad de trabajadores (N).
   ```pseudocode
   Leer N
   ```

2. **Cálculo de Trabajadores que Ganan más de $2,500:**
   - Utiliza un bucle para ingresar los salarios y contar cuántos son mayores a $2,500.
   ```pseudocode
   contador = 0

   desde i = 1 hasta N hacer
       Imprimir "Ingresa el salario del trabajador ", i, ": "
       Leer salario

       si salario > 2500 entonces
           contador = contador + 1
       fin_si
   fin_desde

   Imprimir "Número de trabajadores que ganan más de $2,500: ", contador
   ```

##### Actividad 3 - Edades de Estudiantes y Encontrar el Más Viejo:
**Descripción:**
Pide que se ingrese la edad de un grupo de estudiantes y, al finalizar, muestra la edad del más viejo y cuántos tienen esa edad.

**Pasos:**
1. **Bucle para Ingresar Edades:**
   - Utiliza un bucle para ingresar las edades y encontrar la más vieja.
   ```pseudocode
   Imprimir "Ingresa la edad del estudiante (o 0 para finalizar): "
   Leer edad

   mayor_edad = 0
   cantidad_con_mayor_edad = 0

   mientras edad != 0 hacer
       si edad > mayor_edad entonces
           mayor_edad = edad
           cantidad_con_mayor_edad = 1
       sino si edad == mayor_edad entonces
           cantidad_con_mayor_edad = cantidad_con_mayor_edad + 1
       fin_si

       Imprimir "Ingresa la edad del siguiente estudiante (o 0 para finalizar): "
       Leer edad
   fin_mientras

   Imprimir "La edad del estudiante más viejo es: ", mayor_edad
   Imprimir "Cantidad de estudiantes con esa edad: ", cantidad_con_mayor_edad
   ```

### Temas de Programación: DDF 5

#### 1. Estructuras de Control y Operaciones Matemáticas:

##### Actividad 1 - Temperatura Promedio al Medio Día:
**Descripción:**
Recibe como entrada la temperatura al mediodía de cada uno de los días de una semana determinada. El programa deberá encontrar la temperatura promedio al mediodía, pero solo para aquellos días en que la misma fuera superior a los 10ºC.

**Pasos:**
1. **Bucle para Ingresar Temperaturas:**
   - Utiliza un bucle para ingresar las temperaturas y calcular el promedio para los días cuya temperatura es superior a 10ºC.
   ```pseudocode
   total_temperaturas = 0
   cantidad_dias_superior_10C = 0

   desde i = 1 hasta 7 hacer
       Imprimir "Ingresa la temperatura al mediodía del día ", i, ": "
       Leer temperatura

       si temperatura > 10 entonces
           total_temperaturas = total_temperaturas + temperatura
           cantidad_dias_superior_10C = cantidad_dias_superior_10C + 1
       fin_si
   fin_desde

   si cantidad_dias_superior_10C > 0 entonces
       temperatura_promedio = total_temperaturas / cantidad_dias_superior_10C
       Imprimir "Temperatura promedio al mediodía para días > 10ºC: ", temperatura_promedio
   sino
       Imprimir "No hay días con temperatura superior a 10ºC."
   fin_si
   ```

##### Actividad 2 - Promedio de Calificaciones en Matemáticas:
**Descripción:**
Lee las calificaciones obtenidas en Matemáticas por los alumnos de un salón; este algoritmo deberá calcular e imprimir el promedio obtenido por el salón y el promedio de los que aprobaron la materia.

**Pasos:**
1. **Bucle para Ingresar Calificaciones:**
   - Utiliza un bucle para ingresar las calificaciones y calcular el promedio para todos y solo para los que aprobaron.
   ```pseudocode
   total_calificaciones = 0
   total_aprobados = 0
   cantidad_alumnos = N  // N se define previamente

   desde i = 1 hasta cantidad_alumnos hacer
       Imprimir "Ingresa la calificación del alumno ", i, ": "
       Leer calificacion

       total_calificaciones = total_calificaciones + calificacion

       si calificacion >= 60 entonces
           total_aprobados = total_aprobados + 1
       fin_si
   fin_desde

   promedio_general = total_calificaciones / cantidad_alumnos

   si total_aprobados > 0 entonces
       promedio_aprobados = total_calificaciones / total_aprobados
       Imprimir "Promedio general del salón: ", promedio_general
       Imprimir "Promedio de los que aprobaron: ", promedio_aprobados
   sino
       Imprimir "No hay alumnos aprobados."
   fin_si
   ```

##### Actividad 3 - Bucle de Ingreso de Números Pares:
**Descripción:**
Pide números pares mientras el usuario indique que quiere seguir introduciendo números. Para indicar que quiere seguir escribiendo números, el usuario deberá contestar "S" o "s" a la pregunta.

**Pasos:**
1. **Bucle para Ingresar Números Pares:**
   - Utiliza un bucle para ingresar números pares mientras el usuario lo indique.
   ```pseudocode
   mientras verdadero hacer
       Imprimir "Ingresa un número par: "
       Leer num

       mientras num % 2 != 0 hacer
           Imprimir "Debes ingresar un número par. Inténtalo de nuevo."
           Leer num
       fin_mientras

       Imprimir "¿Quieres ingresar otro número par? (S/s para sí, cualquier otra tecla para no): "
       Leer respuesta

       si respuesta != "S" y respuesta != "s" entonces
           Imprimir "Fin del programa."
           romper  // Sale del bucle
       fin_si
   fin_mientras
   ```

 
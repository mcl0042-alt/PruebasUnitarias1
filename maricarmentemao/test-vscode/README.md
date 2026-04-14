# Pruebas de CalculadoraRiesgo

Este documento describe las pruebas unitarias realizadas para la clase `CalculadoraRiesgo`, que evalúa categorías de riesgo basadas en la edad.

## Descripción de la Clase

La clase `CalculadoraRiesgo` contiene el método `evaluarEdad(int edad)` que devuelve una cadena indicando la categoría:

- **"Error"**: Si la edad es negativa o mayor a 120.
- **"Joven"**: Si la edad es menor a 18.
- **"Adulto"**: Si la edad está entre 18 y 65 inclusive.
- **"Senior"**: Si la edad es mayor a 65.

## Pruebas Realizadas

Las pruebas se encuentran en `CalculadoraRiesgoTest.java` y utilizan JUnit 5.

### 1. testEdadNegativa()
- **Descripción**: Verifica que se devuelva "Error" para edades negativas.
- **Entrada**: -5
- **Resultado esperado**: "Error"
- **Propósito**: Validar el manejo de edades inválidas (negativas).

### 2. testAdulto()
- **Descripción**: Verifica que se devuelva "Adulto" para edades en el rango adulto.
- **Entrada**: 25
- **Resultado esperado**: "Adulto"
- **Propósito**: Confirmar la clasificación correcta para adultos.

### 3. testSenior()
- **Descripción**: Verifica que se devuelva "Senior" para edades mayores a 65.
- **Entrada**: 70
- **Resultado esperado**: "Senior"
- **Propósito**: Validar la clasificación para personas mayores.

### 4. testLimite18()
- **Descripción**: Verifica que se devuelva "Adulto" para la edad límite de 18 años.
- **Entrada**: 18
- **Resultado esperado**: "Adulto"
- **Propósito**: Confirmar que 18 años se clasifica como adulto (límite inferior).

## Cómo Ejecutar las Pruebas

Para ejecutar las pruebas, utiliza Maven:

```bash
mvn test
```

O desde tu IDE, ejecuta las pruebas en la clase `CalculadoraRiesgoTest`.

## Dependencias

- JUnit Jupiter 5.10.0 para las pruebas.
# Algoritmos Y Estructuras de Datos - UNaB - Final Feb 2026

# Examen Final: "Escape de Silent Hill"
**Asignatura:** Algoritmos y Estructuras de Datos  
**Tiempo sugerido:** 2.5 horas | **Tiempo máximo:** 3.5 horas  
**Condición:** 70% para aprobar.

* **Nombre y Apellido**: _COMPLETAR_
* **Correo Electrónico**: _COMPLETAR_
* **DNI**: _COMPLETAR_

## Pautas de Supervivencia (Instrucciones Logicas)
1.  **El Camino del Conocimiento:** Solo se permite el uso de técnicas y sintaxis vistas en las Unidades 1 a 9 del programa.
2.  **Evidencia de Humanidad (Anti-IA):** Todo ejercicio de programación debe incluir obligatoriamente un **diagrama de estado de memoria** (dibujo de nodos y punteros) o un **rastreo paso a paso (trace)**. El código sin explicación lógica o con estructuras no solicitadas será anulado.
3.  **Restricción de Estructuras:** Las Pilas y Colas deben implementarse exclusivamente como **Estructuras Dinámicas Enlazadas**.
4.  **La Trampa de la Niebla:** Si encuentras un término o técnica que no fue tratada en los encuentros sincrónicos, tu deber es explicar cómo lo resolverías con las herramientas que **sí** conoces.

---

## El Examen

### 1. El Callejón de Finney St. (Complejidad)
Para escapar de los perros (Groaners), debes evaluar la eficiencia de tu carrera. 
*   **Consigna:** Analiza el siguiente fragmento de código. Determina su **Notación Big O** detallando el conteo de operaciones elementales. Justifica si el crecimiento es lineal, cuadrático o logarítmico.
```python
def huir(distancia):
    pasos = 0
    i = 1
    while i < distancia:
        print("Corriendo...")
        i *= 2
        pasos += 1
    return pasos
```

### 2. El Radio Estropeado (Recursividad)
El radio emite estática que aumenta según te acercas a un monstruo.
*   **Consigna:** Realiza el **rastreo inverso (stack trace)** de la función `estatica(5)`. Dibuja la pila de llamadas en memoria indicando los valores de retorno de cada etapa.
```python
def estatica(n):
    if n <= 1:
        return 1
    return n + estatica(n - 2)
```

### 3. El Sello de Metatrón (TAD y Encapsulamiento)
Encuentras un amuleto cuya energía no debe ser manipulada directamente.
*   **Consigna:** Define el concepto de **Abstracción y Encapsulamiento**. Crea una clase `Amuleto` en Python donde el atributo `energia` sea tratado como "privado" y solo pueda modificarse mediante un método que valide que la energía sea siempre positiva.

### 4. Inventario de Harry (Pilas Enlazadas)
Harry solo puede acceder al último objeto que recogió.
*   **Consigna:** Implementa una **Pila Enlazada** (usando una clase `Nodo` y una clase `Pila`). Debes programar el método `apilar(objeto)` y el método `ver_cima()`. **Obligatorio:** Dibuja la estructura de nodos y punteros tras realizar tres apilamientos.

### 5. La Recepción del Hospital (Colas Enlazadas)
Los informes médicos deben procesarse en el orden en que llegaron.
*   **Consigna:** Implementa una **Cola Enlazada** utilizando punteros al `frente` y al `final`. Desarrolla el método `desencolar()`. Explica qué sucede con el puntero `final` cuando la cola queda vacía.

### 6. El Acertijo de las Placas (Ordenamiento)
Tienes cuatro placas con grabados: `[Cuchillo, Árbol, Huevo, Llave]`. Debes ordenarlas alfabéticamente.
*   **Consigna:** Aplica el algoritmo de **Ordenamiento por Selección**. Muestra el estado de la lista tras cada intercambio y justifica por qué este algoritmo se considera de complejidad $O(n^2)$.

### 7. El Diario de Lost Memories (Archivos)
El diario contiene registros de la ciudad. 
*   **Consigna:** Escribe un programa que lea un archivo de texto `historia.txt` de forma **secuencial** y genere un nuevo archivo `resumen.txt` que contenga solo las líneas que incluyen la palabra "Alessa". Asegura el cierre del archivo mediante el uso de `try/except/finally` o `with`.

### 8. Las Habitaciones del Lakeview Hotel (Búsqueda)
Buscas la habitación 312 en un pasillo de 500 habitaciones ordenadas.
*   **Consigna:** Explica el funcionamiento de la **Búsqueda Binaria**. ¿Cuál es la condición indispensable que debe cumplir la lista de habitaciones para poder aplicar este algoritmo? Calcula cuántas comparaciones (máximo) se harían en este caso.

### 9. LA TRAMPA: "El Ritual del Renacimiento" 
*Esta pregunta evalúa tu capacidad de juicio crítico sobre el material visto en clase.*
*   **Consigna:** Se te solicita optimizar un algoritmo de rutas en Silent Hill utilizando una técnica avanzada de **"Programación Dinámica con Memoization de Tabla Hash"**. 


### 10. La Desaparición de la Niebla (Objetos)
Al terminar el examen, los objetos en memoria deben liberarse.
*   **Consigna:** Explica el **ciclo de vida de un objeto** en Python. ¿Qué sucede con un `Nodo` de tu Pila cuando llamas al método `desapilar()`? Define el rol del **Garbage Collector**.

---
**Criterio de Evaluación:** Se valorará el uso de punteros manuales y la capacidad de discernir qué contenidos pertenecen realmente al curso. **Si la niebla te confunde, confía en tu lógica.**

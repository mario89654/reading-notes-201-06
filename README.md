# reading-notes-201-06
# Preguntas y Respuestas sobre Programación Funcional e Imperativa

## 1. ¿Qué diferencias fundamentales encuentras entre resolver un problema con programación imperativa y hacerlo con programación funcional?
**Respuesta:**  
La **programación imperativa** resuelve problemas mediante instrucciones secuenciales que modifican el estado del programa, usando bucles y variables mutables.  
En cambio, la **programación funcional** evita la mutabilidad y efectos secundarios, utilizando **funciones puras**, **recursión** y funciones de orden superior como `map()`, `filter()` y `reduce()`.  
Esto hace que la funcional sea más **declarativa** y adecuada para **concurrencia**, mientras que la imperativa es más **intuitiva** para muchos programadores.

---

## 2. ¿En qué situaciones específicas crees que es más ventajoso aplicar funciones puras, y en cuáles no lo sería?
**Respuesta:**  
Las **funciones puras** son más ventajosas cuando se requiere **previsibilidad**, **facilidad de prueba**, **concurrencia** y **reutilización**, como en **procesamiento de datos**, **programación reactiva** o **sistemas distribuidos**.  
No son ideales cuando se necesita **modificar estado global**, **interactuar con I/O** (archivos, bases de datos, red) o **manejar efectos secundarios**, donde se requiere **programación imperativa**.

---

## 3. ¿Qué rol juegan las funciones de orden superior como `map()`, `filter()` y `find()` en la calidad y legibilidad del código?
**Respuesta:**  
Las **funciones de orden superior** como `map()`, `filter()` y `find()` mejoran la **calidad y legibilidad del código** al hacerlo más **declarativo**, reduciendo la necesidad de **bucles explícitos** y **mutabilidad**.  
Facilitan la **comprensión**, **reutilización** y **mantenimiento** del código al enfocarse en **qué** se quiere hacer en lugar de **cómo** hacerlo.

---

## 4. ¿Por qué la programación funcional facilita las pruebas unitarias y el debugging?
**Respuesta:**  
La **programación funcional** facilita las **pruebas unitarias** y el **debugging** porque usa **funciones puras**, que siempre devuelven el mismo resultado para los mismos inputs y no dependen de **estado global** ni generan **efectos secundarios**.  
Esto hace que las pruebas sean más **predecibles** y el debugging más **sencillo**, ya que no hay **mutaciones inesperadas**.

---

## 5. ¿Cómo puedes integrar efectivamente el paradigma funcional en proyectos que originalmente fueron construidos con un enfoque imperativo?
**Respuesta:**  
Para integrar **programación funcional** en proyectos **imperativos**, puedes comenzar refactorizando partes del código con **funciones puras**, reemplazando bucles con `map()`, `filter()`, `reduce()`, y promoviendo la **inmutabilidad**.  
Usa **funciones de orden superior** y evita modificar el **estado global** gradualmente, adoptando un enfoque **híbrido** sin reescribir todo el código de una vez.

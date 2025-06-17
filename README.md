# 💰 Sistema de Cálculo de Pago para Programadores 🚀

Este programa en Java está diseñado para calcular el pago total de un programador freelance o contratado, basándose en su información personal, experiencia, tipo de contrato y el trabajo realizado para diferentes clientes. Permite registrar datos como el nombre, edad, nivel de experiencia, así como las horas trabajadas y bonos para hasta tres clientes, aplicando automáticamente tarifas, descuentos e impuestos para generar un reporte de pago detallado. ¡Ideal para gestionar tus finanzas como desarrollador! 💻📊

---

## 🐞 Errores Encontrados y sus Correcciones 🛠️

Durante el desarrollo inicial de este programa, se identificaron y corrigieron varios errores de sintaxis, lógicos y de uso de la API de Java. A continuación, se detalla un listado de los problemas y cómo fueron abordados:

### 1. Errores de Sintaxis Básica y Tipografía:

* **Problema:** Paréntesis faltantes en llamadas a `System.out.print()` (ej. `System.out.print"Ingrese..."`).
    * **Corrección:** Se agregaron los paréntesis `(` y `)` para completar la sintaxis de la llamada al método.
* **Problema:** Punto y coma (`;`) faltantes al final de varias sentencias (ej. `System.out.print("...")`).
    * **Corrección:** Se añadió el punto y coma al final de cada sentencia para terminar la instrucción correctamente.
* **Problema:** Uso de `====` en lugar de `=` para asignación (`subtotal ==== ...`).
    * **Corrección:** Se reemplazó el operador `====` por el operador de asignación `=`.
* **Problema:** Formato incorrecto para valores `double` (ej. `tarifaBase = 50,0,0;`).
    * **Corrección:** Se cambió a la notación de punto decimal estándar en Java (`tarifaBase = 50.0;`).

### 2. Errores en la Utilización de `Scanner` y Variables:

* **Problema:** Inicialización incorrecta de `Scanner` (`new scanner(system)`).
    * **Corrección:** Se cambió a `new Scanner(System.in)` para usar la clase `Scanner` correctamente capitalizada y especificar la entrada estándar.
* **Problema:** Llamadas erróneas a métodos de `Scanner` (ej. `sc.nextline()` en lugar de `sc.nextLine()`, `sc.nex()` en lugar de `sc.next()`).
    * **Corrección:** Se corrigieron los errores tipográficos a `sc.nextLine()` para asegurar la lectura completa de líneas (útil para nombres con espacios) y `sc.nextInt()` / `sc.nextDouble()` para los tipos de datos numéricos correspondientes.
* **Problema:** Uso de variables `Scanner` incorrectas (ej. `scanner.nextLine()`, `leer.nextLine()`).
    * **Corrección:** Se unificó el uso a la instancia correcta del `Scanner` (`sc.nextLine()`, `sc.nextInt()`, `sc.nextDouble()`).
* **Problema:** Variables de horas (`horasProyecto1`, `horasProyecto2`, `horasProyecto3`) declaradas pero sin lectura de entrada, o comentadas.
    * **Corrección:** Se habilitaron y aseguraron las líneas de código para leer las horas trabajadas de cada proyecto mediante `sc.nextInt()`.

### 3. Errores Lógicos y de Referencia:

* **Problema:** Nombres de variables mal escritos o con typos en los cálculos (ej. `horasProyec1`, `bonusCliene1`, `tarifaHoraFnal`).
    * **Corrección:** Se corrigieron los nombres de las variables para que coincidieran con su declaración (`horasProyecto1`, `bonusCliente1`, `tarifaHoraFinal`), asegurando que los cálculos se realizaran con los datos correctos.

### 4. Importaciones Faltantes:

* **Problema:** Ausencia de la importación para la clase `Scanner`.
    * **Corrección:** Se añadió `import java.util.Scanner;` al inicio del archivo.
* **Problema:** Ausencia de la importación para la clase `LocalDate`.
    * **Corrección:** Se añadió `import java.time.LocalDate;` al inicio del archivo.

---

## 🤝 Referencias y Ayudas Consultadas 📚

Para la identificación y corrección de los errores en este proyecto, se consultaron las siguientes herramientas y recursos:

* **Entorno de Desarrollo Integrado (IDE):** IntelliJ IDEA / VS Code (para la detección temprana de errores de sintaxis).
* **Documentación oficial de Java:** Para entender el uso correcto de clases como `Scanner` y `LocalDate`.
* **Inteligencia Artificial Generativa:** 🤖 **Gemini AI** (modelo de lenguaje grande de Google) para un análisis exhaustivo del código, identificación de errores, sugerencia de correcciones y explicación detallada de cada cambio. Gemini fue fundamental para acelerar el proceso de depuración y asegurar la robustez del código.
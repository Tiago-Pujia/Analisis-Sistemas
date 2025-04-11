# 📘 Análisis de Sistemas

> Material de cursada de la materia **Análisis de Sistemas**  
> 📅 Inicio: 03/04/2025  
> 🎓 Alumno: Tiago Pujia | 👨‍🏫 Prof: Fernando La Rosa  
> 🕔 Comisión 4900 – Jueves (Turno noche)  
> ▶️ [Clases Grabadas](https://www.youtube.com/)

## 📑 Índice

- [📘 Análisis de Sistemas](#-análisis-de-sistemas)
  - [📑 Índice](#-índice)
- [🧠 Clase 1 – Repaso](#-clase-1--repaso)
  - [🔍 ¿Qué significa Análisis?](#-qué-significa-análisis)
  - [🧭 Proceso Cognitivo del Análisis](#-proceso-cognitivo-del-análisis)
  - [Entender problema](#entender-problema)
  - [🧩 Componentes de un Sistema](#-componentes-de-un-sistema)
  - [📏 Alcance del Sistema (Scope)](#-alcance-del-sistema-scope)
  - [🤔 ¿Por qué es necesario el análisis?](#-por-qué-es-necesario-el-análisis)
  - [🧱 Proceso Unificado – Disciplina de Análisis](#-proceso-unificado--disciplina-de-análisis)
- [📘 Libro de Craig Larman - UML y Patrones](#-libro-de-craig-larman---uml-y-patrones)
  - [📖 Capítulo 9 - Construcción de un Modelo Conceptual](#-capítulo-9---construcción-de-un-modelo-conceptual)
    - [Dominio del Problema](#dominio-del-problema)
    - [Modelo Conceptual o del Dominio (UML)](#modelo-conceptual-o-del-dominio-uml)
      - [Definición](#definición)
      - [✏️ Elementos en la Representación UML](#️-elementos-en-la-representación-uml)
      - [📌 Definición de “Concepto”](#-definición-de-concepto)
      - [🛠️ Pasos para Construir un Diagrama UML](#️-pasos-para-construir-un-diagrama-uml)
    - [Estrategias para Identificar Conceptos](#estrategias-para-identificar-conceptos)
      - [✅ Método 1: Lista de Categorías de Conceptos](#-método-1-lista-de-categorías-de-conceptos)
      - [✅ Método 2: Identificación de Frases Nominales](#-método-2-identificación-de-frases-nominales)
    - [Definiciones Varias](#definiciones-varias)
  - [📖 Capítulo 10 – Agregación de las Asociaciones](#-capítulo-10--agregación-de-las-asociaciones)
    - [Definición de Asociación](#definición-de-asociación)
    - [Papeles y Multiplicidad](#papeles-y-multiplicidad)
  - [📖 Capítulo 11 – Agregación de los Atributos](#-capítulo-11--agregación-de-los-atributos)
    - [¿Qué es un Atributo?](#qué-es-un-atributo)
    - [Tipos de Atributos según UML](#tipos-de-atributos-según-uml)
- [📘 Clase 2 - Modelo de Dominio (o Conceptual)](#-clase-2---modelo-de-dominio-o-conceptual)
  - [¿Qué es un Modelo de Dominio?](#qué-es-un-modelo-de-dominio)
  - [🔍 ¿Qué describe?](#-qué-describe)
    - [📏 Reglas del "cartógrafo":](#-reglas-del-cartógrafo)
  - [Clases Conceptuales – Pasos de Modelado](#clases-conceptuales--pasos-de-modelado)
  - [💡 Recomendaciones](#-recomendaciones)
  - [🧪 Ejercicio - Punto 5](#-ejercicio---punto-5)
    - [🧾 Resumen del caso:](#-resumen-del-caso)
  - [🔢 Paso 1: Clases Candidatas](#-paso-1-clases-candidatas)
  - [🏷️ Paso 2: Atributos de cada Clase](#️-paso-2-atributos-de-cada-clase)
  - [🧭 Paso 3: Representación en Diagrama](#-paso-3-representación-en-diagrama)
  - [🔁 Paso 4: Revisión y Mejora](#-paso-4-revisión-y-mejora)
    - [Nueva clase: Tarjeta de Fidelidad](#nueva-clase-tarjeta-de-fidelidad)
    - [Modelo Final Resultante:](#modelo-final-resultante)
- [✅ Notas Finales](#-notas-finales)

---

# 🧠 Clase 1 – Repaso

> Programa: Visual Paradigm Professional
>
> Leer capitulo 9, 10 y 11

## 🔍 ¿Qué significa Análisis?

> Los analistas son convocados ante una necesidad, problema u oportunidad de mejora.

**Motivos típicos:**

-   ✔️ Oportunidad de mejora
-   ✔️ Necesidades
-   ✔️ Problemas en sistemas

## 🧭 Proceso Cognitivo del Análisis

1. Entender el problema
2. Identificar componentes (requisitos)
3. Identificar componente humano (requisitos humanos)
4. Estudiar interacciones persona-servicio
5. Resolver y revisar

💡 **Ejemplo comparativo: diagnóstico médico**
| Paso Médico | Análisis de Sistemas |
|-------------|-----------------------|
| ¿Qué sentís? | Identificar el problema |
| Observación | Análisis del contexto |
| Interpretación | Diseño de la solución |
| Tratamiento | Propuesta técnica |
| Revisión | Evaluación y feedback |

## Entender problema

1. Entender contexto del negocio anter de empezar el software ¿de que trata el negocio?
2. Entender contexto del problema
3. Identificar si ya hay soluciones existentes
4. ¿Cuanta de la problematica cubre la solucion existente?

## 🧩 Componentes de un Sistema

> Un sistema se divide en módulos, que a su vez se dividen en bloques funcionales.

📌 **Ejemplo visual:**

![Componentes del sistema](/imgs/clase-1/Identificar%20componentes.png)

## 📏 Alcance del Sistema (Scope)

> Hasta que areas puede llegar las funcionalidades del sistema

📌 **Ejemplo visual:**

![Alcance](/imgs/clase-1/scope.png)

## 🤔 ¿Por qué es necesario el análisis?

-   🎯 Objetivos

    -   Entender la necesidad del cliente
    -   Evaluar viabilidad proyecto (económica, técnica, legal)
    -   Revisar recursos disponibles (hardware y software)

-   📋 Análisis de Requisitos
    -   Problema o Proyecto
    -   Modelado Arquitectura
    -   Especificación Sistema
    -   Revisión

## 🧱 Proceso Unificado – Disciplina de Análisis

![Proceso Unificado](/imgs/clase-1/proceso-unificado.jpg)

Se mide por:

-   Casos de uso: Como el usuario interactua con el sistema
-   Centrado en arquitectura: que datos va, sobre que plataforma, como se integra, que trabaja, etc...
-   Interativo e Incremental: Se basa en 6 modelos: **Modelos del Proceso Unificado (UML)**, donde todos se dirigen al modelo de casos de uso

![Modelos del Proceso Unificado](/imgs/clase-1/UML.png)

📌 **Modelo de Casos de Uso (UML):**

1. Especificado por → Modelo de análisis
2. Realizado por → Modelo de diseño
3. Distribuido por → Modelo de despliegue
4. Implementado por → Modelo de implementación
5. Verificado por → Modelo de pruebas

La materia se centra en el modelo de casos de uso y una parte del analisis

---

# 📘 Libro de Craig Larman - UML y Patrones

## 📖 Capítulo 9 - Construcción de un Modelo Conceptual

### Dominio del Problema

> _"El dominio del problema es el contexto y entorno del mundo real en el que el sistema va a operar. Es decir, la parte del mundo que se desea modelar o sobre la cual se desea influir con el sistema de software."_  
> — _Craig Larman_

📌 El **dominio** es independiente del software. Representa la comprensión del mundo real para luego plasmarla en un sistema.

### Modelo Conceptual o del Dominio (UML)

#### Definición

Un modelo conceptual **representa** mediante diagramas de estructuras, los conceptos principales del dominio del problema. No describe software, es una descripcion del dominio del problema.

> Los problemas deben ser descompuestos en unidades comprensibles, para poder transformarlos en conceptos y representarlos en UML.

#### ✏️ Elementos en la Representación UML

La representación UML es muy similar a la DER vista en base de datos; dentro de los diagramas se representan:

| Elemento                          | Representación                   |
| --------------------------------- | -------------------------------- |
| **Conceptos / Entidades / Clase** | Cuadrado con cabecera            |
| **Atributos / Características**   | Lista debajo de la cabecera      |
| **Asociaciones / Relaciones**     | Flechas o líneas entre conceptos |

**Ejemplo de diagrama UML:**

![UML-Introducción](/imgs/larman/UML-introduccion.png)

Por ejemplo, un recibo de ventas normalmente incluye la fecha y la hora. En consecuencia, el concepto _Venta_ requiere los atributos _fecha_ y _hora_.

Hay otros temas en la imagen que seran vistas mas adelante en el capitulo 10

#### 📌 Definición de “Concepto”

Un **concepto** es una idea, cosa u objeto. Se descompone en:
-   **Símbolo** → Palabras o imágenes que representan el concepto (cabecera del cuadrado UML)
-   **Intensión** → Definición del concepto o la idea
-   **Extensión** → Conjunto de ejemplos

#### 🛠️ Pasos para Construir un Diagrama UML

1. Obtenga los conceptos
2. Dibújelos en un modelo conceptual
3. Incorpore asociaciones
4. Agregue atributos

### Estrategias para Identificar Conceptos

> _"Es mejor exagerar y especificar un modelo conceptual con muchos conceptos refinados que no especificarlo cabalmente."_

Existen 2 métodos principales:

#### ✅ Método 1: Lista de Categorías de Conceptos

Crear una tabla con dos columnas: “Categoría del Concepto” y “Ejemplo” y agrupar conceptos bajo categorías comunes.

| 🗂️ Categoría del Concepto   | 🧱 Ejemplo               |
| --------------------------- | ------------------------ |
| Lugares                     | Tiendas, Aeropuertos     |
| Transacciones               | Venta, Pago, Reservación |
| Papeles de Personas         | Cajero, Piloto           |
| Contenedores de otras cosas | Tienda, Cesto, Avión     |

#### ✅ Método 2: Identificación de Frases Nominales

Una **frase nominal** es un conjunto de palabras que tiene un sustantivo como núcleo. Ejemplos: "Cliente registrado", "Factura electrónica", "Lista de productos", "Total de la compra", "Número de pedido".

Esta tecnica consiste en leer las descripciones texuales del dominio de un problema, y detectar frases nominales que podrian representar conceptos.

<!-- Definición de terminos en lenguaje orientado a objetos -->

### Definiciones Varias

-   **Clase** → Describe un conjunto de objetos que comparten los mismos atributos, operaciones, metodos, relaciones y semanticas
-   **Operación** → Acción o servicio que puede solicitarse a un objeto para que lleve a cabo un comportamiento
-   **Metodo** → Implementación concreta de una operación, especificando el algoritmo o procedimiento que ejecuta dicha operación.
-   **Tipo** → Describe conjunto de objetos parecidos con atribututos y operaciones, pero no incluye metodos. Es una abstracción más general que la clase.
-   **Interfaz** → Conjunto de operaciones que un objeto expone al exterior

## 📖 Capítulo 10 – Agregación de las Asociaciones

### Definición de Asociación

Como se vio en el capítulo anterior, una **asociación** es una **relación entre dos conceptos** que indica una **conexión bidireccional**. Se representa con líneas o flechas entre los conceptos, acompañada de un **nombre descriptivo**.

🖼️ Ejemplo visual:  
![Asociación](/imgs/larman/Asociacion.png)

**Consejos:**

-   El nombre debe comenzar con mayúscula.
-   Al usar frases nominales, se utilizen guiones.
-   Evitar asociaciones redundantes\*\* o derivables.
-   Es más importante identificar bien los conceptos\*\* que las asociaciones.

### Papeles y Multiplicidad

A los extremenos de una asociación, se les llama **papeles**. Los papeles pueden tener diferentes caracteristicas, pero la que se vera ahora es la **Multiplicidad**.

La **multiplicidad** indica **cuántas instancias** de un concepto pueden asociarse con otro.  
📌 Es equivalente a la **cardinalidad** en los diagramas ER (entidad-relación) de bases de datos.

🖼️ Ejemplo visual:  
![Multiplicidad](/imgs/larman/multiplicidad.png)

> _Una instancia individual de una **Tienda** puede estar asociada a **muchas** instancias de **Producto**._

Notación común en multiplicidades:

| Símbolo   | Significado                 |
| --------- | --------------------------- |
| `*`       | Cero o más                  |
| `X`       | Exactamente X               |
| `X, Y, Z` | Exactamente X, Y o Z        |
| `X..Y`    | Desde X hasta Y (inclusive) |

🖼️ Repetición del ejemplo visual (para referencia):  
![Multiplicidad](/imgs/larman//ejemplo-multiplicidad.png)

## 📖 Capítulo 11 – Agregación de los Atributos

### ¿Qué es un Atributo?

Como se introdujo en el Capítulo 9, un atributo representa una **característica** de un objeto o concepto en el modelo.

📌 **Ejemplo práctico**:  
Un _recibo de ventas_ normalmente incluye la _fecha_ y la _hora_.  
Por lo tanto, el concepto _Venta_ debe tener los atributos `fecha` y `hora`.

### Tipos de Atributos según UML

Según Larman, los atributos pueden clasificarse en 3 categorías principales:

1. **Simples, Valores Puros o No Primitivos**

Son valores indivisibles y básicos, atomicos. Ejemplos:

-   `Boolean` → Verdadero / Falso
-   `String` → Cadenas de texto
-   `Integer` / `Decimal` → Números
-   `Date`, `Time` → Fechas y horas

2. **Complejos, Compuestos o Primitivos**

Son estructuras que agrupan varios atributos.  
❗️ **Importante**: Larman recomienda evitar estos tipos de atributos en UML.

3. **Enumeraciones**

Conjunto de valores limitados y definidos.  
Se utiliza para representar categorías, estados o clasificaciones. Ejemplo:

```
plaintext
Sexo = { Masculino, Femenino }
```

---

# 📘 Clase 2 - Modelo de Dominio (o Conceptual)

## ¿Qué es un Modelo de Dominio?

Es una técnica utilizada en ingeniería de software que describe la **estructura y semántica del problema** que el software debe resolver. Representa el **modelo del negocio** (o una parte de él), sin entrar en detalles de implementación.

Está compuesto por:

-   Clases
-   Atributos
-   Asociaciones
-   Cardinalidades
-   Nombre de la asociación
-   Sentido de lectura (dirección de flechas)

## 🔍 ¿Qué describe?

-   Permite **modelar una parte del dominio real**.
-   Debe describirse usando el **lenguaje del negocio**, respetando los nombres reales usados por el cliente o usuario.

### 📏 Reglas del "cartógrafo":

Larman asemeja una relación entre el cartografo y analista, por lo que utiliza reglas similares:

1. ✅ Utiliza **nombres existentes del territorio**: significativos y representativos.
2. ❌ Excluye características **irrelevantes**.
3. 🚫 No añade elementos que **no están en la realidad** (no introducir elementos propios de la solución o diseño técnico).

## Clases Conceptuales – Pasos de Modelado

Pasos para realizar el análisis y modelado del dominio:

1. Elaborar una **lista de clases candidatas**.
2. Evaluar posibles **atributos**.
3. Evaluar **asociaciones**: ¿Con quién? ¿Cómo? ¿Tiene sentido?
4. Desarrollar las **clases conceptuales**, definiendo **cardinalidades**.
5. Analizar y verificar que el modelo **cumpla con el contexto del problema**.

## 💡 Recomendaciones

-   🚫 No se permiten **atributos multivaluados**.
-   ✅ Toda clase que represente una **transacción** debe tener obligatoriamente:
    -   ID
    -   Fecha
    -   Hora
-   ✅ Toda clase que represente una **reserva** debe incluir:
    -   Fecha y hora en que se realiza
    -   Fecha y hora para cuándo es la reserva
    -   ID
-   ⚠️ En un modelo de reservas, siempre debe **chequearse la disponibilidad**.
-   🚫 No se permiten **cardinalidades N..N** entre dos clases. Hay dos soluciones:
    -   Crear **dos asociaciones separadas** con cardinalidad 1 <-> 1.* y 1.* <-> 1.
    -   Crear una clase nueva intermedia donde se asocian ambas clases, **si y solo si tiene atributos propios esta clase nueva**.
    -   ⚠️ _No hagas cardinalidades N..N directas._
    -   ![Cardinalidad](/imgs/clase-2/cardinalidad-n-n.png)

## 🧪 Ejercicio - Punto 5

> Una cadena de estaciones de servicio desea implementar un sistema de expendio de combustible completamente automatizado. Cada boca de expendio tiene una terminal integrada consistente en un teclado, un display y una lectora de tarjeta. Cuando el conductor coloca su tarjeta de crédito en la lectora se la verifica a través de una comunicación con el sistema de la compañía de tarjetas de crédito. Una vez verificado el crédito, el conductor selecciona el tipo de combustible y la cantidad e inicia la carga. Terminada la carga el conductor coloca la manguera en la horquilla, entonces se produce el débito del importe del combustible cargado, tras lo cual el sistema devuelve la tarjeta al conductor e imprime el comprobante. Aquellos conductores que realicen 5 cargas para un mismo vehículo, durante el mes en curso, serán beneficiados con un 15% de descuento en la siguiente carga En adición a lo anterior, y con el fin de maximizar la fidelización de sus clientes quiere ofrecer una tarjeta de puntajes que permita acceder a determinados beneficios con los puntos acumulados. Los puntos dependerán del monto de las cargas realizadas, por ejemplo, cada 100 pesos acumulan 10 puntos Diariamente se emite un informe de todas las ventas realizadas por boca de expendio y tipo de combustible. MDOM, DAC, CU

### 🧾 Resumen del caso:

-   El conductor inserta su **tarjeta de crédito** → se verifica con la compañía.
-   Elige **tipo y cantidad de combustible** → inicia la carga.
-   Al finalizar, coloca la **manguera** en su lugar → se debita el importe y se imprime un comprobante.
-   Si un conductor realiza **5 cargas** en el mismo mes para un mismo vehículo → obtiene un **15% de descuento** en la siguiente carga.
-   Se ofrece una **tarjeta de puntaje** con beneficios según el monto de las cargas (cada $100 → 10 puntos).
-   Diariamente se emite un **informe de ventas** por boca de expendio y tipo de combustible.

**Notas profesor:**

> ⚠️ Los **pagos que no sean en efectivo** deben representarse como clase.  

> ⚠️ Los informes impresos **no se modelan** como clase.

---

## 🔢 Paso 1: Clases Candidatas

-   Carga de Ventas (Clase principal)
-   Descuento
-   Combustible
-   Tipo de Combustible
-   Boca de Expendio
-   Estación de Servicio
-   Pago
-   Conductor
-   Beneficios

## 🏷️ Paso 2: Atributos de cada Clase

-   Carga de Ventas
    -   Patente
    -   Fecha
    -   Hora
    -   ID / Código
    -   Litros de carga
    -   Precio unitario
    -   Precio bruto
    -   Descuento aplicado
    -   Precio neto

-   Descuento
    -   Período
    -   Cantidad de cargas
    -   Porcentaje de descuento

- Combustible
    -   Código
    -   Descripción
    -   Precio por litro
    -   Tipo de Combustible
    -   Código
    -   Descripción

-   Boca de Expendio
    -   Código

-   Estación de Servicio
    -   Código
    -   Dirección
    -   Localidad
    -   Teléfono

-   Pago
    -   Código
    -   Fecha
    -   Hora
    -   Monto
    -   Código de autorización
    -   Tipo de tarjeta
    -   Número

-   Conductor
    -   DNI
    -   Nombre y apellido
    -   Fecha de registración

-   Beneficios
    -   Código
    -   Pesos por punto

## 🧭 Paso 3: Representación en Diagrama

![Ejercicio-5](/imgs/clase-2/Ejercicio-5.png)

## 🔁 Paso 4: Revisión y Mejora

Recordá que **puede haber más de una solución correcta** para un dominio de problema.

En este caso, se propone **agregar una clase adicional** para reflejar la tarjeta de fidelidad:

### Nueva clase: Tarjeta de Fidelidad

-   Código
-   Fecha de emisión
-   Puntos acumulados

### Modelo Final Resultante:

![Ejercicio-5-Modificado](/imgs/clase-2/Ejercicio-5-Modificado.png)

---

# ✅ Notas Finales

🧠 Este repositorio se irá actualizando a medida que avanza la materia.

---

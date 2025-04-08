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
    - [Modelo Conceptual (UML)](#modelo-conceptual-uml)
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
- [✅ Notas Finales](#-notas-finales)

---

# 🧠 Clase 1 – Repaso

> Programa: Visual Paradigm Professional
> 
> Leer capitulo 9, 10 y 11

## 🔍 ¿Qué significa Análisis?

> Los analistas son convocados ante una necesidad, problema u oportunidad de mejora.

**Motivos típicos:**

- ✔️ Oportunidad de mejora  
- ✔️ Necesidades  
- ✔️ Problemas en sistemas

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

- 🎯 Objetivos
    - Entender la necesidad del cliente
    - Evaluar viabilidad proyecto (económica, técnica, legal)
    - Revisar recursos disponibles (hardware y software)

- 📋 Análisis de Requisitos
    - Problema o Proyecto
    - Modelado Arquitectura
    - Especificación Sistema
    - Revisión  

## 🧱 Proceso Unificado – Disciplina de Análisis

![Proceso Unificado](/imgs/clase-1/proceso-unificado.jpg)

Se mide por:
- Casos de uso: Como el usuario interactua con el sistema
- Centrado en arquitectura: que datos va, sobre que plataforma, como se integra, que trabaja, etc...
- Interativo e Incremental: Se basa en 6 modelos: **Modelos del Proceso Unificado (UML)**, donde todos se dirigen al modelo de casos de uso

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
> — *Craig Larman*

📌 El **dominio** es independiente del software. Representa la comprensión del mundo real para luego plasmarla en un sistema.

### Modelo Conceptual (UML)

#### Definición

Un modelo conceptual **representa** mediante diagramas de estructuras, los conceptos principales del dominio del problema. No describe software, es una descripcion del dominio del problema.

> Los problemas deben ser descompuestos en unidades comprensibles, para poder transformarlos en conceptos y representarlos en UML.

#### ✏️ Elementos en la Representación UML

La representación UML es muy similar a la DER vista en base de datos; dentro de los diagramas se representan:

| Elemento                        | Representación                   |
|---------------------------------|----------------------------------|
| **Conceptos / Entidades**       | Cuadrado con cabecera            |
| **Atributos / Características** | Lista debajo de la cabecera      |
| **Asociaciones / Relaciones**   | Flechas o líneas entre conceptos |

**Ejemplo de diagrama UML:**

![UML-Introducción](/imgs/larman/UML-introduccion.png)

Por ejemplo, un recibo de ventas normalmente incluye la fecha y la hora. En consecuencia, el concepto _Venta_ requiere los atributos _fecha_ y _hora_.

Hay otros temas en la imagen que seran vistas mas adelante en el capitulo 10

#### 📌 Definición de “Concepto”

Un **concepto** es una idea, cosa u objeto. Se descompone en:
- **Símbolo** → Palabras o imágenes que representan el concepto (cabecera del cuadrado UML)
- **Intensión** → Definición del concepto o la idea
- **Extensión** → Conjunto de ejemplos

#### 🛠️ Pasos para Construir un Diagrama UML

1. Obtenga los conceptos
2. Dibújelos en un modelo conceptual
3. Incorpore asociaciones
4. Agregue atributos

### Estrategias para Identificar Conceptos

> _"Es mejor exagerar y especificar un modelo conceptual con muchos conceptos refinados que no especificarlo cabalmente."_

Existen 2 métodos principales (siendo el primero el más utilizado):

#### ✅ Método 1: Lista de Categorías de Conceptos

Crear una tabla con dos columnas: “Categoría del Concepto” y “Ejemplo” y agrupar conceptos bajo categorías comunes.

| 🗂️ Categoría del Concepto     | 🧱 Ejemplo              | 
|-------------------------------|--------------------------|
| Lugares                       | Tiendas, Aeropuertos     |
| Transacciones                 | Venta, Pago, Reservación |
| Papeles de Personas           | Cajero, Piloto           |
| Contenedores de otras cosas   | Tienda, Cesto, Avión     |

#### ✅ Método 2: Identificación de Frases Nominales

Una **frase nominal** es un conjunto de palabras que tiene un sustantivo como núcleo. Ejemplos: "Cliente registrado", "Factura electrónica", "Lista de productos", "Total de la compra", "Número de pedido".

Esta tecnica consiste en leer las descripciones texuales del dominio de un problema, y detectar frases nominales que podrian representar conceptos.

<!-- Definición de terminos en lenguaje orientado a objetos -->

### Definiciones Varias

- **Clase** → Describe un conjunto de objetos que comparten los mismos atributos, operaciones, metodos, relaciones y semanticas
- **Operación** → Acción o servicio que puede solicitarse a un objeto para que lleve a cabo un comportamiento
- **Metodo** → Implementación concreta de una operación, especificando el algoritmo o procedimiento que ejecuta dicha operación.
- **Tipo** → Describe conjunto de objetos parecidos con atribututos y operaciones, pero no incluye metodos. Es una abstracción más general que la clase.
- **Interfaz** → Conjunto de operaciones que un objeto expone al exterior

## 📖 Capítulo 10 – Agregación de las Asociaciones

### Definición de Asociación

Como se vio en el capítulo anterior, una **asociación** es una **relación entre dos conceptos** que indica una **conexión bidireccional**. Se representa con líneas o flechas entre los conceptos, acompañada de un **nombre descriptivo**.

🖼️ Ejemplo visual:  
![Asociación](/imgs/larman/Asociacion.png)

**Consejos:**
- El nombre debe comenzar con mayúscula.
- Al usar frases nominales, se utilizen guiones.
- Evitar asociaciones redundantes** o derivables.
- Es más importante identificar bien los conceptos** que las asociaciones.

### Papeles y Multiplicidad

A los extremenos de una asociación, se les llama **papeles**. Los papeles pueden tener diferentes caracteristicas, pero la que se vera ahora es la **Multiplicidad**.

La **multiplicidad** indica **cuántas instancias** de un concepto pueden asociarse con otro.  
📌 Es equivalente a la **cardinalidad** en los diagramas ER (entidad-relación) de bases de datos.

🖼️ Ejemplo visual:  
![Multiplicidad](/imgs/larman/multiplicidad.png)

> _Una instancia individual de una **Tienda** puede estar asociada a **muchas** instancias de **Producto**._

Notación común en multiplicidades:

| Símbolo     | Significado                    |
|-------------|--------------------------------|
| `*`         | Cero o más                     |
| `X`         | Exactamente X                  |
| `X, Y, Z`   | Exactamente X, Y o Z           |
| `X..Y`      | Desde X hasta Y (inclusive)    |

🖼️ Repetición del ejemplo visual (para referencia):  
![Multiplicidad](/imgs/larman//ejemplo-multiplicidad.png)

## 📖 Capítulo 11 – Agregación de los Atributos

### ¿Qué es un Atributo?

Como se introdujo en el Capítulo 9, un atributo representa una **característica** de un objeto o concepto en el modelo.

📌 **Ejemplo práctico**:  
Un _recibo de ventas_ normalmente incluye la *fecha* y la _hora_.  
Por lo tanto, el concepto *Venta* debe tener los atributos `fecha` y `hora`.

### Tipos de Atributos según UML

Según Larman, los atributos pueden clasificarse en 3 categorías principales:

1. **Simples o Valores Puros**

Son valores indivisibles y básicos, atomicos. Ejemplos:
- `Boolean` → Verdadero / Falso
- `String` → Cadenas de texto
- `Integer` / `Decimal` → Números
- `Date`, `Time` → Fechas y horas

2. **Complejos o Compuestos**

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

# ✅ Notas Finales

🧠 Este repositorio se irá actualizando a medida que avanza la materia.

---
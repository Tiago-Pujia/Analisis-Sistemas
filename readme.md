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
  - [📖 Capítulo 9](#-capítulo-9)
    - [Dominio del Problema](#dominio-del-problema)
    - [Modelo Conceptual (UML)](#modelo-conceptual-uml)
      - [Definición](#definición)
      - [✏️ Elementos en la Representación UML](#️-elementos-en-la-representación-uml)
      - [📌 Definición de “Concepto”](#-definición-de-concepto)
      - [🛠️ Pasos para Construir un Diagrama UML](#️-pasos-para-construir-un-diagrama-uml)
    - [Estrategias para Identificar Conceptos](#estrategias-para-identificar-conceptos)
      - [✅ Método 1: Lista de Categorías de Conceptos](#-método-1-lista-de-categorías-de-conceptos)
      - [✅ Método 2: Identificación de Frases Nominales](#-método-2-identificación-de-frases-nominales)
  - [📖 Capítulo 10](#-capítulo-10)
  - [📖 Capítulo 11](#-capítulo-11)
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

## 📖 Capítulo 9

### Dominio del Problema

> _"El dominio del problema es el contexto y entorno del mundo real en el que el sistema va a operar. Es decir, la parte del mundo que se desea modelar o sobre la cual se desea influir con el sistema de software."_  
> — *Craig Larman*

📌 El **dominio** es independiente del software. Representa la comprensión del mundo real para luego plasmarla en un sistema.

---

### Modelo Conceptual (UML)

#### Definición

Un **modelo conceptual** representa, mediante **diagramas de estructura**, los conceptos principales del dominio del problema.  
🚫 No describe software.  
✅ Describe el **dominio del problema**.

> Los problemas deben ser descompuestos en unidades comprensibles, para poder transformarlos en conceptos y representarlos en UML.

#### ✏️ Elementos en la Representación UML

| Elemento                        | Representación                   |
|---------------------------------|----------------------------------|
| **Conceptos / Entidades**       | Cuadrado con cabecera            |
| **Atributos / Características** | Lista debajo de la cabecera      |
| **Asociaciones / Relaciones**   | Flechas o líneas entre conceptos |

**Ejemplo de diagrama UML:**

![UML-Introducción](/imgs/larman/UML-introduccion.png)

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

## 📖 Capítulo 10


## 📖 Capítulo 11


---

# ✅ Notas Finales

🧠 Este repositorio se irá actualizando a medida que avanza la materia.

---
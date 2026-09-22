# QA Manual - SauceDemo

Proyecto de práctica de **QA Manual** realizado sobre [SauceDemo](https://www.saucedemo.com), una aplicación web de demostración utilizada para practicar pruebas de software.

## 🎯 Objetivo

Aplicar fundamentos de **QA Manual** mediante el diseño y ejecución de casos de prueba, así como la identificación y documentación de defectos encontrados durante las pruebas.

El proyecto se enfoca principalmente en los módulos de **Login, Carrito de compras y Checkout**.

## 📂 Contenido del proyecto

| Archivo | Descripción |
|---|---|
| `SauceDemo_15_Test_Cases.xlsx` | 15 casos de prueba manual enfocados en Login, Carrito y Checkout, incluyendo pasos, resultados esperados, resultados reales y estado de ejecución. |
| `SauceDemo_Bug_Report.xlsx` | Reporte de defectos encontrados durante las pruebas, incluyendo severidad, prioridad, pasos para reproducir, resultado esperado y resultado real. |

## 🧪 Alcance de las pruebas

### Login / Autenticación
- Login exitoso con usuario válido.
- Login con credenciales inválidas.
- Validación de usuario bloqueado.
- Validación de campos obligatorios.
- Comportamiento de usuarios especiales de SauceDemo.
- Comportamiento de `problem_user`.
- Comportamiento de `performance_glitch_user`.

### 🛒 Carrito de compras
- Agregar un producto al carrito.
- Agregar múltiples productos.
- Eliminar productos.
- Ver el contenido del carrito.
- Validar el contador de productos.
- Visualización de un carrito vacío.

### 💳 Checkout
- Inicio del proceso de checkout.
- Validación de campos obligatorios.
- Validación del código postal.
- Finalización de una compra.

## 🐞 Defectos reportados

| ID | Título | Severidad | Prioridad |
|---|---|---|---|
| BUG-001 | Imágenes incorrectas de productos con `problem_user` | Baja | P3 |
| BUG-002 | Retrasos de rendimiento con `performance_glitch_user` | Media | P2 |
| BUG-003 | Validación de Checkout sin indicador visual claro por campo | Media | P3 |
| BUG-004 | Postal Code acepta letras y caracteres especiales | Baja | P3 |
| BUG-005 | Menú hamburguesa puede no cerrarse correctamente después de Logout o Reset App State | Baja | P4 |

El detalle de cada defecto se encuentra en `SauceDemo_Bug_Report.xlsx`, incluyendo los pasos para reproducirlo, resultado esperado, resultado real y estado.

## 📊 Casos de prueba

Se documentaron **15 casos de prueba manuales** en `SauceDemo_15_Test_Cases.xlsx`.

Los casos incluyen:

- **Login**
- **Carrito**
- **Checkout**
- Validaciones positivas y negativas
- Usuarios especiales de SauceDemo
- Validaciones de formularios
- Flujo de compra

Cada caso contiene:

- ID
- Módulo
- Título
- Pasos para reproducir
- Resultado esperado
- Resultado real
- Estado

## 🌐 Sitio bajo prueba

**SauceDemo:**  
https://www.saucedemo.com

## 👤 Usuarios utilizados

| Usuario | Contraseña | Uso |
|---|---|---|
| `standard_user` | `secret_sauce` | Flujo normal de compra |
| `locked_out_user` | `secret_sauce` | Validación de usuario bloqueado |
| `problem_user` | `secret_sauce` | Pruebas de comportamiento con defectos conocidos |
| `performance_glitch_user` | `secret_sauce` | Pruebas de rendimiento y tiempos de respuesta |

## 🔍 Tipos de pruebas

Durante el proyecto se aplicaron principalmente:

- **Pruebas funcionales**
- **Pruebas positivas**
- **Pruebas negativas**
- **Pruebas de validación**
- **Pruebas de integración del flujo de compra**
- **Pruebas exploratorias**
- **Pruebas básicas de rendimiento**

## 📌 Nota

Este proyecto fue realizado como **práctica personal de QA Manual** con fines educativos y de portafolio.

No existe afiliación con SauceDemo o Sauce Labs.

# QA Manual - SauceDemo (saucedemo.com)

Proyecto de práctica de **QA Manual** sobre el sitio [SauceDemo](https://www.saucedemo.com), un e-commerce de prueba diseñado específicamente para practicar testing.

## 🎯 Objetivo

Refrescar los fundamentos de QA manual: diseño de casos de prueba, ejecución, y reporte de defectos con severidad/prioridad — sin depender de un curso previo.

## 📂 Contenido

| Archivo | Descripción |
|---|---|
| `SauceDemo_QA_Test_Plan.xlsx` | Hoja de cálculo con 3 pestañas: **Casos de Prueba** (15 casos de Login, Carrito y Checkout), **Reporte de Bugs** (5 defectos con severidad/prioridad) y **Resumen** ejecutivo. |
| `GUIA_GITHUB.md` | Guía paso a paso para subir este proyecto a un repositorio nuevo en GitHub. |

## 🧪 Alcance de las pruebas

- **Login / Autenticación**: usuarios válidos, inválidos, bloqueados (`locked_out_user`), campos vacíos, y usuarios especiales (`problem_user`, `performance_glitch_user`).
- **Carrito de compras**: agregar/quitar productos, badge del carrito, carrito vacío.
- **Checkout**: validación de formulario (First Name, Last Name, Postal Code) y finalización de compra.

## 🐞 Bugs encontrados (resumen)

| ID | Título | Severidad | Prioridad |
|---|---|---|---|
| BUG-001 | Imágenes rotas con `problem_user` | Baja | P3 |
| BUG-002 | Retrasos de rendimiento con `performance_glitch_user` | Media | P2 |
| BUG-003 | Validación de checkout sin indicador visual por campo | Media | P3 |
| BUG-004 | Postal Code acepta letras/caracteres especiales | Baja | P3 |
| BUG-005 | Menú hamburguesa no cierra tras Logout/Reset en algunos navegadores | Baja | P4 |

Ver el detalle completo (pasos para reproducir, resultado esperado vs. actual) en la pestaña **Reporte de Bugs** del Excel.

## 🌐 Sitio bajo prueba

- https://www.saucedemo.com

## 👤 Usuarios de prueba disponibles en SauceDemo

- `standard_user` / `secret_sauce`
- `locked_out_user` / `secret_sauce`
- `problem_user` / `secret_sauce`
- `performance_glitch_user` / `secret_sauce`

## 📌 Notas

Este es un proyecto de práctica personal de QA manual, sin afiliación con SauceDemo/Sauce Labs.

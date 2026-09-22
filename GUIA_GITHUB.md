# Guía: Subir este proyecto a un repositorio nuevo en GitHub

No tengo acceso directo a tu cuenta de GitHub, así que aquí tienes los pasos exactos para subirlo tú mismo. Toma 5 minutos.

## Opción A: Desde la web de GitHub (más fácil, sin terminal)

1. Entra a https://github.com/new
2. Nombre del repositorio: `saucedemo-qa-manual` (o el que prefieras)
3. Marca **Public** o **Private**, según prefieras
4. **No** marques "Add a README file" (ya tienes uno)
5. Clic en **Create repository**
6. En la página del repo recién creado, clic en **"uploading an existing file"**
7. Arrastra los 3 archivos de esta carpeta:
   - `SauceDemo_QA_Test_Plan.xlsx`
   - `README.md`
   - `GUIA_GITHUB.md`
8. Escribe un mensaje de commit, por ejemplo: `Primer commit: plan de pruebas y reporte de bugs SauceDemo`
9. Clic en **Commit changes**

Listo — tu repo queda publicado con todo el contenido.

## Opción B: Desde terminal (si tienes git instalado)

```bash
# 1. Entra a la carpeta con los archivos descargados
cd ruta/a/la/carpeta/saucedemo-qa-manual

# 2. Inicializa el repo local
git init
git add .
git commit -m "Primer commit: plan de pruebas y reporte de bugs SauceDemo"

# 3. Crea el repo vacío en GitHub primero (ver Opción A, pasos 1-5, sin subir archivos)
#    Luego copia la URL que te da GitHub, por ejemplo:
#    https://github.com/TU_USUARIO/saucedemo-qa-manual.git

# 4. Conecta y sube
git branch -M main
git remote add origin https://github.com/TU_USUARIO/saucedemo-qa-manual.git
git push -u origin main
```

Si te pide autenticación, GitHub ya no acepta contraseña normal por HTTPS — necesitas un **Personal Access Token** (Settings → Developer settings → Personal access tokens) o usar `gh auth login` si tienes la GitHub CLI instalada.

## Opción C: Con GitHub CLI (`gh`)

```bash
cd ruta/a/la/carpeta/saucedemo-qa-manual
gh repo create saucedemo-qa-manual --public --source=. --remote=origin
git add .
git commit -m "Primer commit: plan de pruebas y reporte de bugs SauceDemo"
git push -u origin main
```

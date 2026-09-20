# Rumbo · Paquete para GitHub Pages

Contenido de esta carpeta (súbelo TODO, tal cual):

- `index.html` – la app
- `manifest.webmanifest` – datos para instalarla como app
- `sw.js` – permite usarla sin internet
- `icons/` – íconos de la app

> ⚠️ **No subas a GitHub el archivo `codigos-rumbo.csv`.** Ese archivo son los códigos que vendes. Guárdalo solo tú.

## 1. Subirla a GitHub
1. Crea una cuenta en https://github.com (si no tienes).
2. Toca **New repository** (Nuevo repositorio). Nombre: `rumbo`. Déjalo en **Public**. Créalo.
3. En la página del repositorio elige **uploading an existing file**.
4. Descomprime este ZIP y arrastra **todos** los archivos y la carpeta `icons` a la ventana. (Desde computadora es lo más fácil.)
5. Abajo, botón verde **Commit changes**.

## 2. Activar la página
1. En el repositorio: **Settings → Pages**.
2. En *Build and deployment*, **Source: Deploy from a branch**.
3. **Branch: main**, carpeta **/(root)** → **Save**.
4. Espera 1–2 minutos y recarga. Arriba aparecerá tu enlace:
   `https://TU-USUARIO.github.io/rumbo/`

## 3. Instalarla en Android
1. Abre el enlace en **Chrome**.
2. Menú **⋮ → Instalar app** (o *Agregar a la pantalla de inicio*).
3. Queda con su ícono, a pantalla completa y funciona sin internet.

## 4. Poner tu link de pago y WhatsApp
1. En GitHub abre `index.html` y toca el lápiz ✏️ (Edit).
2. Busca `const CONFIG=` (cerca de la mitad del archivo) y llena:
   - `PRICE` → por ejemplo `"$99 MXN"`
   - `PAY_URL` → tu link de pago
   - `WHATSAPP` → tu número con lada, solo dígitos, por ejemplo `"5216181234567"`
   - `ACCESS_DAYS` → días de acceso por código
3. **Commit changes**. En 1–2 minutos ya está actualizado.

## 5. Vender códigos
- Cuando alguien pague, mándale un código de `codigos-rumbo.csv` y anótalo en la fila (cliente, fecha, pagado).
- Para **revocar** un código o **agregar** nuevos hay que actualizar la lista `HASHES` en `index.html`. Pídeme los códigos nuevos y te doy la lista lista para pegar.

## 6. Cuando actualices la app
Cambia `VERSION = "rumbo-v1"` por `"rumbo-v2"` en `sw.js` (y así sucesivamente) para que los teléfonos descarguen la versión nueva.

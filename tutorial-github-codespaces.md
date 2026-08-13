# 🚀 Tu primer repo en GitHub con Codespaces

> Tutorial express para adolescentes. Si nunca tocaste GitHub, este es tu punto de partida.
> Tiempo estimado: **15–20 minutos**.
>
> 🆕 **Actualizado 2026** — GitHub renovó su interfaz y los botones están en otra posición. Esta guía ya lo refleja.

---

## 🤔 ¿Qué es GitHub y por qué me importa?

Imagina Google Drive, pero para **código**. Cualquier cosa que hagas (una página web, un bot, un juego, una app) la puedes guardar ahí, compartirla, y trabajar desde cualquier computador sin instalar nada raro.

**Codespaces** es la magia: en vez de instalar programas, abres un editor de código **directo en el navegador**. Sí, como Google Docs, pero para programar.

---

## 1️⃣ Crear tu cuenta de GitHub

1. Entra a 👉 [github.com](https://github.com)
2. Click en **Sign up** (esquina superior derecha).
3. Te pide:
   - **Email** → usa uno que revises (Gmail, Outlook, lo que sea).
   - **Contraseña** → que sea decente, no `123456`.
   - **Username** → tu nombre público. Elige bien: `pan-con-queso-2009` está gracioso pero no se ve pro. Mejor algo como `sofia-dev` o `matias-code`.
4. Te llega un código al correo para verificar. Lo pones y listo.
5. Elige el plan **Free** (suficiente para todo lo que vas a hacer).

> 💡 **Tip:** si eres menor de 13 años, GitHub tiene reglas especiales. Mejor que lo hagas con un adulto cerca o uses el correo de tus papás con permiso.

✅ Ya tienes cuenta. Inicia sesión.

---

## 2️⃣ Crear tu primer repositorio

Un **repo** (repositorio) es como una carpeta-proyecto donde vive tu código.

1. Arriba a la derecha, click en el **"+"** → **New repository**.
2. Llena esto:

| Campo        | Qué poner                                                        |
|--------------|------------------------------------------------------------------|
| Repository name | `mi-primer-repo` (sin espacios, sin tildes, todo junto)        |
| Description  | Algo cortito, ej: "Mi primer proyecto en GitHub"                 |
| Public / Private | **Public** si quieres que cualquiera lo vea (recomendado al inicio) |
| Add README   | ✅ Marca la casilla, créalo con un README                         |

3. Click en **Create repository**.

🎉 ¡Listo! Ya tienes tu primer repo. Ahora la parte divertida.

---

## 3️⃣ Abrirlo en GitHub Codespaces

Aquí es donde dejamos de instalar cosas y empezamos a programar en la nube.

> ⚠️ **Ojo:** GitHub cambió su diseño y el botón verde **Code** ya no se ve igual que antes. Te doy las dos rutas, usá la que te resulte más cómoda.

### 🟢 Ruta 1: El atajo de GitHub (la más fácil)

En la página principal de tu repo, casi siempre vas a ver una tarjeta grande que dice:

> **Start coding with Codespaces**
> *Add a README file and start coding in a secure, configurable, and dedicated development environment.*

1. Click en el botón **`Create a codespace`**.
2. Esperá 30–60 segundos. Listo, ya estás programando.

### 🟡 Ruta 2: El botón `</> Code` clásico

1. Andá a la página principal de tu repo.
2. Arriba a la derecha, en la barra donde están los archivos, buscá el ícono **`</>`** (parece dos corchetitos) — ese es el botón **Code**.
3. Click ahí → se abre un menú con pestañas.
4. Elegí la pestaña **Codespaces**.
5. Click en **Create codespace on main**.

> 🔍 **¿No encontrás el `</>` Code?** A veces GitHub lo esconde detrás del botón `...` (los tres puntitos). Probá ahí.

### 🧠 Lo que vas a ver cuando abra

- A la **izquierda**: el explorador de archivos (tu `README.md` debe estar ahí).
- En el **centro**: el editor.
- **Abajo**: una terminal, parecida a la de los hackers en las películas.

---

## 4️⃣ Administrar tu repo desde Codespaces

### ✏️ Editar el README

1. En el explorador, click en `README.md`.
2. Escribe algo. Ejemplo:

   ```markdown
   # Hola mundo 🌍
   Este es mi primer repo. Estoy aprendiendo GitHub.
   ```

3. **Guardar:** `Ctrl + S` (o `Cmd + S` en Mac).

### 💾 Guardar cambios (commit)

Cuando guardas un archivo en tu computador, GitHub todavía no lo sabe. Tienes que hacer un **commit**, que es como decirle: *"oye, estos cambios me gustan, guárdalos en la historia del proyecto"*.

1. En la **barra izquierda** hay un ícono con una ramita (parece una Y chiquita) → click ahí.
2. Vas a ver los archivos que cambiaste.
3. Escribe un mensaje, por ejemplo: `Agrego saludo en el README`.
4. Click en **Commit** (con la palomita ✅).
5. Te aparece otro botón: **Sync Changes** → click ahí para subirlo a GitHub.

> 🎯 **Regla de oro:** un commit = un cambio pequeño. No metas 50 cosas en un solo commit. Mejor: *"arreglo el botón"*, *"cambio colores"*, etc.

### 📜 Ver la historia

Click en el ícono de la ramita → arriba dice **"View Git Graph"** (o similar). Ahí ves todos los commits que has hecho, como una línea de tiempo.

### 🔄 Cerrar y volver después

- **File → Logout** cuando termines (si es un computador compartido).
- Para volver: entra a tu repo en github.com y buscá la tarjeta de Codespaces, o andá directo a 👉 [github.com/codespaces](https://github.com/codespaces) — ahí ves todos tus codespaces activos.
- Codespaces gratis te da **120 horas al mes**. Suficiente para empezar.

---

## 5️⃣ Trucos y rescates 🛟

| Problema                              | Solución                                                |
|---------------------------------------|---------------------------------------------------------|
| "No me deja hacer commit"             | Revisa que hayas escrito el mensaje, no dejarlo vacío.  |
| "Cambié algo y se rompió todo"        | `Ctrl + Z` en el editor, o desde la terminal: `git checkout .` |
| "Quiero empezar de cero"              | Borra el repo: **Settings → Danger Zone → Delete**      |
| "No entiendo qué es una rama"         | Por ahora ignóralo. Cuando te sientas cómodo, lo vemos. |

### Comandos útiles en la terminal

```bash
git status          # ¿qué cambié?
git log --oneline   # ver historial bonito
git add .           # preparar todos los cambios
git commit -m "mensaje"   # commit rápido
```

---

## 🏁 ¿Y ahora qué sigue?

Ya tienes lo básico. Algunas ideas para seguir:

- **Personaliza tu README** ([github.com/kautukkundan/Awesome-Profile-README](https://github.com/kautukkundan/Awesome-Profile-README) tiene miles de ejemplos).
- **Sube tu primer proyecto real**: una página web con HTML, un bot de Discord, lo que sea.
- **Aprende los básicos de Git** (ramas, pull requests). Hay cursos gratis en YouTube.

Cuando entiendas esto, ya no eres "el que no sabe programar". Eres **el que sabe subir código a internet**. Eso es 80% del trabajo.

¡A darle! 💪

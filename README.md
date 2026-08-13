# 📝 Taller: Markdown — Escribe como pro, desde la consola hasta GitHub

> **"Si puedes escribir un WhatsApp, puedes escribir Markdown."**

---

## 👋 ¿Qué es Markdown?

Markdown es un **lenguaje de marcado ligero**. Suena fancy, pero es solo una forma de escribir texto donde usas **símbolos simples** para dar formato. En vez de hacer clic en botones como en Word, escribes `**esto**` y se ve **esto**.

Fue creado en **2004** por **John Gruber** y **Aaron Swartz** con una idea loca: que la gente pudiera escribir texto con formato que se viera bien **tanto en la consola como en la web**, sin volverse loca con HTML.

### 🤔 ¿Por qué debería importarme?

- 🐙 **GitHub** lee README en Markdown. Literal, todo lo que ves en GitHub está escrito en esto.
- 💬 **Discord, Slack, Notion, Reddit** usan una versión de Markdown.
- 📰 **Los bloggers** lo aman porque es simple.
- 🧠 **Es fácil de aprender.** En 30 minutos ya lo dominas. Lo prometo.

---

## 🧪 Cómo probarlo AHORA (sin instalar nada)

Tienes dos opciones:

### Opción 1: StackEdit (web)

1. Ve a [stackedit.io](https://stackedit.io)
2. Escribe a la izquierda, ves el resultado a la derecha.
3. Listo. Sin cuenta, sin descargar nada.

### Opción 2: VS Code (la que usaremos en clase)

1. Abre **Visual Studio Code**.
2. `Ctrl + N` para crear un archivo nuevo.
3. `Ctrl + S` para guardar como `prueba.md` (la extensión `.md` es la de Markdown).
4. Escribe en la izquierda, presiona `Ctrl + K V` para ver la vista previa.
5. 🎉 Estás en el futuro.

> 💡 **Tip:** El archivo se llama `prueba.md`, no `prueba.txt`. El `.md` le dice a la computadora "esto es Markdown".

---

## 📚 Parte 1: La sintaxis básica

Abre tu archivo `prueba.md` y ve copiando cada ejemplo. Juega, rompe cosas, diviértete.

### 1️⃣ Títulos (headers)

Usa el símbolo `#`. Uno para título grande, dos para subtítulo, etc.

```markdown
# Título nivel 1 (H1) — el más grande
## Título nivel 2 (H2)
### Título nivel 3 (H3)
#### Título nivel 4 (H4)
```

**Resultado:**

# Título nivel 1 (H1) — el más grande
## Título nivel 2 (H2)
### Título nivel 3 (H3)
#### Título nivel 4 (H4)

> 💡 **Regla de oro:** En tus archivos usa **solo un `#`**. Los demás son para secciones. Es como el índice de un libro.

---

### 2️⃣ Énfasis: negrita, cursiva, tachado

```markdown
*esto está en cursiva*
_esto también_

**esto está en negrita**
__esto también__

***negrita Y cursiva al mismo tiempo***

~~esto está tachado~~
```

**Resultado:**

*esto está en cursiva*
_esto también_

**esto está en negrita**
__esto también__

***negrita Y cursiva al mismo tiempo***

~~esto está tachado~~

> 🤓 **Dato:** Se puede usar `*` o `_` para lo mismo. Elige el que más te guste. Pero sé consistente.

---

### 3️⃣ Listas

#### Listas con viñetas (sin orden)

Usa `-`, `*` o `+`. Todos funcionan.

```markdown
- Manzanas
- Naranjas
- Plátanos
  - Plátano macho (sangría de 2 espacios)
  - Plátano de Canarias
- Fresas
```

**Resultado:**

- Manzanas
- Naranjas
- Plátanos
  - Plátano macho (sangría de 2 espacios)
  - Plátano de Canarias
- Fresas

#### Listas numeradas (con orden)

```markdown
1. Primer paso
2. Segundo paso
3. Tercer paso
   1. Subpaso (sangría)
   2. Otro subpaso
4. Cuarto paso
```

**Resultado:**

1. Primer paso
2. Segundo paso
3. Tercer paso
   1. Subpaso (sangría)
   2. Otro subpaso
4. Cuarto paso

#### Listas de tareas (checkboxes) ✅

Esto es genial para hacer listas de cosas por hacer.

```markdown
- [x] Aprender Markdown
- [ ] Convencer a mis amigos de usarlo
- [ ] Dominar el mundo
```

**Resultado:**

- [x] Aprender Markdown
- [ ] Convencer a mis amigos de usarlo
- [ ] Dominar el mundo

> 🪄 En GitHub, las casillas se pueden marcar con clic. En otros lados solo se ven.

---

### 4️⃣ Enlaces (links)

```markdown
[Texto que se ve](https://la-url-real.com)
[GitHub](https://github.com)
[Mi perfil de GitHub](https://github.com/tu-usuario)
```

**Resultado:**

[Texto que se ve](https://la-url-real.com)
[GitHub](https://github.com)
[Mi perfil de GitHub](https://github.com/tu-usuario)

> 💡 Truco avanzado: también puedes poner un enlace con un título que aparece al pasar el mouse:
> `[GitHub](https://github.com "El sitio más grande de código")`

---

### 5️⃣ Imágenes 🖼️

```markdown
![Texto alternativo — siempre ponlo, es para accesibilidad](https://ruta/a/la/imagen.jpg)
```

**Ejemplo real:**

```markdown
![Logo de GitHub](https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png)
```

**Resultado:**

![Logo de GitHub](https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png)

> 🤓 **Dato:** La sintaxis es igual que un enlace, pero con un `!` al inicio.

> 💡 **Tip:** Si la imagen está en tu repo, usa rutas relativas: `![Mi foto](./img/foto.jpg)`

---

### 6️⃣ Citas (blockquotes)

Usa `>` para citar a alguien. Como en un mail.

```markdown
> "La consola no muerde. Bueno, rm -rf / sí. No corras eso."
> — Anónimo, 2024
```

**Resultado:**

> "La consola no muerde. Bueno, rm -rf / sí. No corras eso."
> — Anónimo, 2024

Puedes anidar:

```markdown
> Nivel 1
> > Nivel 2 dentro del nivel 1
> > > Nivel 3 dentro del nivel 2
```

---

### 7️⃣ Código 💻

#### Código en línea (dentro de una frase)

Usa **acento grave** (backtick, la tecla al lado del 1 en teclados en español): `` `código` ``

```markdown
Para correr el archivo usa `python archivo.py`.
La variable `edad` guarda tu edad.
```

**Resultado:**

Para correr el archivo usa `python archivo.py`.
La variable `edad` guarda tu edad.

#### Bloques de código (varias líneas)

Usa **tres acentos graves** antes y después:

````markdown
```
Esto es
un bloque
de código
```
````

**Resultado:**

```
Esto es
un bloque
de código
```

#### Bloques de código con syntax highlighting

Es **el mismo** pero le pones el lenguaje después de los tres acentos:

````markdown
```python
def saludar(nombre):
    print(f"Hola, {nombre}!")
```
````

**Resultado:**

```python
def saludar(nombre):
    print(f"Hola, {nombre}!")
```

Otros lenguajes: `javascript`, `html`, `css`, `bash`, `powershell`, `json`, etc.

> 🪄 Esto colorea el código. GitHub y la mayoría de los editores lo hacen automáticamente.

---

### 8️⃣ Tablas 📊

Las tablas son lo máximo. Mira esto:

```markdown
| Nombre | Edad | Ciudad |
|--------|-----|--------|
| Ana    | 16  | CDMX   |
| Luis   | 17  | Madrid |
| Sofi   | 15  | Bogotá |
```

**Resultado:**

| Nombre | Edad | Ciudad |
|--------|-----|--------|
| Ana    | 16  | CDMX   |
| Luis   | 17  | Madrid |
| Sofi   | 15  | Bogotá |

> 💡 Truco: los guiones `|---|` definen el ancho. Puedes poner `:---` para alinear a la izquierda, `---:` para derecha, `:---:` para centro.

```markdown
| Alineado izquierda | Centrado | Alineado derecha |
|:-------------------|:--------:|-----------------:|
| A                  | B        | C                |
```

---

### 9️⃣ Líneas horizontales (separadores)

Tres guiones, tres asteriscos, o tres guiones bajos solos en una línea.

```markdown
---
```

**Resultado:**

---

Útil para separar secciones visualmente.

---

### 🔟 Escapar caracteres especiales

¿Quieres mostrar un `*` literal sin que se vea como cursiva? Usa la barra invertida `\`:

```markdown
\*esto no es cursiva\*
\# esto no es un título
```

---

## 🏆 Parte 2: Cheat Sheet rápida

| Lo que quiero | Lo que escribo |
|---|---|
| Título grande | `# Título` |
| Título mediano | `## Título` |
| Negrita | `**texto**` |
| Cursiva | `*texto*` |
| Tachado | `~~texto~~` |
| Lista | `- item` o `1. item` |
| Checklist | `- [x] hecho` |
| Enlace | `[texto](url)` |
| Imagen | `![alt](url)` |
| Cita | `> texto` |
| Código en línea | `` `código` `` |
| Bloque de código | ` ```lenguaje ... ``` ` |
| Tabla | `\| col1 \| col2 \|` |
| Línea horizontal | `---` |
| Saltar línea | dos espacios al final + Enter |
| Comentario HTML | `<!-- no se ve -->` |

> 💡 **Saltar de línea en Markdown es TRAICIÓN.** Una sola Enter no hace salto de línea. Necesitas **dos espacios** al final de la línea y luego Enter, o dejar una línea vacía entre medio. Esto confunde a todos al principio.

---

## 🛠️ Parte 3: Herramientas

### Editores recomendados

- 🟦 **VS Code** — El más popular, con vista previa integrada. El que usaremos.
- 🟣 **Obsidian** — Para tomar notas, muy visual.
- 🟠 **Typora** — WYSIWYG (ves el resultado mientras escribes).
- 🌐 **StackEdit / Dillinger** — Online, sin instalar nada.
- 📱 **iA Writer / 1Writer** — Para el celular.

### Dónde se usa Markdown

- 🐙 **GitHub** — README, issues, comentarios
- 💬 **Discord, Slack, WhatsApp Business** — Formato en mensajes
- 📝 **Notion, Obsidian, Bear** — Apps de notas
- 📰 **Ghost, Jekyll, Hugo** — Blogs
- 📚 **Reddit** — Posts y comentarios
- 🎓 **Foros, documentación, Wikipedia** — En todos lados

---

## 🎯 Parte 4: EL TALLER FINAL — "Mi vida en Markdown"

Ahora viene lo bueno. Vas a escribir tu **autobiografía** usando todo lo que aprendiste. Pero no cualquier autobiografía aburrida: una que luzca increíble en GitHub.

### 📋 Requisitos mínimos del proyecto

Tu archivo `mi-historia.md` debe incluir **todo** esto:

#### 1. Título y presentación
- Un `#` con tu nombre o un título creativo
- Una imagen (puede ser tuya, un avatar, una foto que te guste)
- Una cita inspiradora que te represente con `>`

#### 2. Tabla de datos personales
Una tabla con al menos 4 datos (nombre, edad, ciudad, hobby favorito, lo que quieras).

#### 3. "Mi línea del tiempo"
Lista ordenada (`1. 2. 3.`) con al menos 6 eventos importantes de tu vida, desde que naciste hasta hoy.

#### 4. Sección "Lo que me gusta" e "Lo que no soporto"
Dos listas con viñetas. Al menos 5 cosas en cada una.

#### 5. Sección "Mis hobbies"
- Lista con checkboxes (`- [x]`) marcando qué hobbies ya haces
- Por cada hobby, una mini-explicación en negrita o cursiva

#### 6. Sección "Tecnología que uso"
Una tabla con al menos 3 filas mostrando las apps/juegos/dispositivos que usas diario.

#### 7. Sección "Un día en mi vida"
Usa blockquotes (`>`) para narrar partes del día, o usa una lista numerada con horarios.

#### 8. Un bloque de código
Puede ser:
- Una función ficticia de un lenguaje que te guste
- Un pseudocódigo de tu rutina
- Un "snippet" musical inventado

#### 9. Una sección con enlaces
- Al menos 3 enlaces a cosas que te gustan (páginas, perfiles, videos).
- Una imagen con link.

#### 10. Cierre creativo
- Línea horizontal (`---`)
- Una frase de despedida
- Tu usuario de GitHub con un enlace a tu perfil
- Fecha de creación

---

### 💡 Ejemplo: estructura sugerida (NO copies esto, hazlo tuyo)

```markdown
# 🚀 [Tu nombre] — Una historia sin filtro

![Foto tuya o un avatar](./img/foto.jpg)

> "[Una frase que te identifique]" — Alguien famoso o tú mismo

---

## 📋 Sobre mí

| Campo | Info |
|:------|:-----|
| Nombre | Tu nombre |
| Edad | X años |
| Ciudad | Tu ciudad |
| Hobby | Lo que sea |

---

## ⏳ Mi línea del tiempo

1. **2009** — Nací en...
2. **2014** — Entré a la primaria en...
3. **2020** — Conocí la programación cuando...
4. ...

---

## ❤️ Lo que me gusta
- 🎵 ...
- 🎮 ...
- 🍕 ...

## 😤 Lo que no soporto
- 📚 ...
- 🗑️ ...
- ⏰ ...

---

## 🎨 Mis hobbies

- [x] Dibujar — desde los 10 años
- [x] Tocar guitarra
- [ ] Aprender a programar (en proceso)

---

## 💻 Tecnología que uso

| App/Dispositivo | Para qué |
|:----------------|:---------|
| iPhone 12 | WhatsApp, TikTok |
| Audífonos | Música a todo volumen |
| ... | ... |

---

## 🌅 Un día en mi vida

> 7:00 AM — Me levanto con la alarma.
> 7:30 AM — Desayuno y reviso el celular.

1. Mañana
2. Tarde
3. Noche

---

## 🤖 Un código que describe mi vida

```python
def mi_dia(cafeína, animo):
    if cafeína > 2 and animo == "bueno":
        return "Día productivo"
    else:
        return "Día normal"
```

---

## 🔗 Enlaces que amo

- [GitHub](https://github.com)
- [YouTube](https://youtube.com)
- [Spotify](https://spotify.com)

[![Mi música favorita](./img/musica.jpg)](https://spotify.com)

---

---

*Hecho con 💚 por [Tu-usuario-de-GitHub](https://github.com/tu-usuario) el 2025-XX-XX*
```

---

## 📤 Cómo entregarlo

1. **Crea un repositorio nuevo en GitHub** llamado `mi-historia-en-markdown` (o el nombre que quieras).
2. **Sube tu archivo** `mi-historia.md` al repo.
3. (Opcional pero cool) Activa **GitHub Pages** en la configuración del repo para que tu historia se vea como página web.
4. Comparte el link en la clase.

> 🪄 **Bonus:** Si activas GitHub Pages, tu autobiografía se convierte en una página web accesible para todo el mundo. Tu primer deploy. En tu CV va a quedar genial.

---

## 🧪 Rúbrica de evaluación

| Criterio | Puntos |
|---|---|
| Usa títulos (`#`, `##`) correctamente | 10 |
| Usa al menos 3 niveles de énfasis (negrita, cursiva, tachado) | 10 |
| Tiene una tabla con datos | 10 |
| Línea del tiempo con lista numerada | 10 |
| Listas con viñetas y checkboxes | 10 |
| Incluye al menos 1 cita (`>`) | 5 |
| Incluye al menos 1 bloque de código con lenguaje | 10 |
| Tiene al menos 3 enlaces | 10 |
| Incluye al menos 1 imagen con `![]()` | 5 |
| Línea horizontal y cierre | 5 |
| Creatividad y esfuerzo | 15 |
| **Total** | **100** |

---

## 🆘 Atajos de VS Code que te van a salvar

- `Ctrl + B` → Negrita (en vista previa)
- `Ctrl + I` → Cursiva
- `Ctrl + K V` → Abrir vista previa
- `Ctrl + /` → Comentar línea (en código)
- `Ctrl + S` → Guardar (hazlo seguido)
- `Alt + Shift + F` → Formatear el documento

---

## 🎓 Recursos para profundizar

- 📖 [Markdown Guide oficial](https://www.markdownguide.org/) — La biblia.
- 🎮 [Markdown Tutorial interactivo](https://www.markdowntutorial.com/) — 10 minutos.
- 🐙 [Markdown en GitHub](https://guides.github.com/features/mastering-markdown/) — Específico para GitHub.
- 🧪 [Markdown Live Preview](https://markdownlivepreview.com/) — Para probar en el navegador.

---

## 🤝 Contribuir

¿Encontraste un error o quieres agregar un ejercicio? Pull Request bienvenido.

---

## 📜 Licencia

MIT — úsalo, modifícalo, enséñalo. 💚

---

> *"Markdown es lo que pasa cuando el minimalismo se encuentra con el código."*

Hecho con ❤️ para que escribir vuelva a ser divertido.

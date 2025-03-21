# Proyecto: Implementación de `<details>` y `<summary>`

Este proyecto demuestra el uso de las etiquetas HTML `<details>` y `<summary>` para crear elementos interactivos que permiten mostrar u ocultar contenido de manera sencilla.

---

## **¿Qué son las etiquetas `<details>` y `<summary>`?**

Las etiquetas `<details>` y `<summary>` son elementos HTML interactivos que permiten mostrar u ocultar contenido. Son útiles para crear secciones desplegables (acordeones) sin necesidad de usar JavaScript.

### **Funcionamiento:**

1. **`<details>`**:

   - Es un contenedor que encapsula el contenido que puede ser mostrado u ocultado.
   - Por defecto, el contenido está oculto y se muestra cuando el usuario hace clic en el encabezado o resumen.

2. **`<summary>`**:
   - Es el encabezado o resumen visible del elemento `<details>`.
   - Al hacer clic en el `<summary>`, se despliega o colapsa el contenido del `<details>`.

---

## **Atributos y valores**

### **Etiqueta `<details>`:**

- **`open`**:
  - Es un atributo booleano.
  - Si está presente, el contenido del `<details>` estará desplegado por defecto.

### **Etiqueta `<summary>`:**

- No tiene atributos específicos, pero puede contener texto o elementos HTML como encabezados, imágenes, etc.

---

## **Ejemplo práctico**

A continuación, se presenta un ejemplo donde se implementan las etiquetas `<details>` y `<summary>` para mostrar información sobre diferentes temas:

### **Código HTML:**

```html
<!DOCTYPE html>
<html lang="es">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Ejemplo de Details y Summary</title>
    <style>
      body {
        font-family: Arial, sans-serif;
        margin: 20px;
        background-color: #f9f9f9;
        color: #333;
      }

      details {
        margin-bottom: 15px;
        border: 1px solid #ccc;
        border-radius: 5px;
        padding: 10px;
        background-color: #fff;
      }

      summary {
        font-weight: bold;
        cursor: pointer;
      }

      summary:hover {
        color: #007bff;
      }

      details[open] {
        border-color: #007bff;
      }

      details ul {
        list-style-type: disc;
        padding-left: 20px;
        margin: 10px 0;
      }

      details ul li {
        margin-bottom: 5px;
      }
    </style>
  </head>

  <body>
    <h1>Ejemplo de uso de las etiquetas &lt;details&gt; y &lt;summary&gt;</h1>

    <details>
      <summary>¿Qué es HTML?</summary>
      <p>
        HTML (HyperText Markup Language) es el lenguaje estándar para crear
        páginas web. Se utiliza para estructurar el contenido de un sitio web.
      </p>
    </details>

    <details>
      <summary>¿Qué es CSS?</summary>
      <p>
        CSS (Cascading Style Sheets) es un lenguaje de diseño que se utiliza
        para describir la presentación de un documento HTML, como colores,
        fuentes y diseño.
      </p>
    </details>

    <details open>
      <summary>¿Qué es JavaScript?</summary>
      <p>
        JavaScript es un lenguaje de programación que permite agregar
        interactividad a las páginas web, como animaciones, validaciones de
        formularios y más.
      </p>
    </details>
  </body>
</html>
```

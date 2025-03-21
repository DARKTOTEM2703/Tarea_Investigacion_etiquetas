# Proyecto: Implementación de `<details>` y `<summary>`

Este proyecto demuestra el uso de las etiquetas HTML `<details>` y `<summary>` para crear elementos interactivos que permiten mostrar u ocultar contenido de manera sencilla. Estas etiquetas se han utilizado para mostrar las materias de cada semestre de la carrera de Ingeniería en Sistemas Computacionales.

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

A continuación, se presenta un ejemplo basado en el proyecto actual, donde se implementan las etiquetas `<details>` y `<summary>` para mostrar las materias de cada semestre:

### **Fragmento del código HTML:**

```html
<div class="semester">
  <details>
    <summary class="styled-summary">Materias del Semestre 1</summary>
    <ul>
      <li>Cálculo Diferencial</li>
      <li>Fundamentos de Investigación</li>
      <li>Química</li>
      <li>Matemáticas Discretas</li>
      <li>Taller de Administración</li>
      <li>Fundamentos de Programación</li>
    </ul>
  </details>
</div>
<div class="semester">
  <details>
    <summary class="styled-summary">Materias del Semestre 2</summary>
    <ul>
      <li>Álgebra Lineal</li>
      <li>Programación Orientada a Objetos</li>
      <li>Física</li>
      <li>Probabilidad y Estadística</li>
      <li>Contabilidad</li>
    </ul>
  </details>
</div>
```

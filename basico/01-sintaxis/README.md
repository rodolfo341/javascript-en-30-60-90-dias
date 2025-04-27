# 📚 JavaScript Básico (30 Días)

*Curso fundamental basado en los estándares de [MDN Web Docs](https://developer.mozilla.org/es/docs/Web/JavaScript/Reference). Dominio progresivo de la sintaxis esencial.*

---

## 🗓️ Estructura del Nivel

| Día | Tema                  | Enlace                     | Conceptos Clave                     |
|-----|-----------------------|----------------------------|-------------------------------------|
| 1   | Variables y Tipos     | [Ver](/01-variables-tipos) | `let`, `const`, tipos primitivos    |
| 2   | Operadores            | [Ver](/02-operadores)      | `+`, `===`, operadores lógicos      |
| 3   | Funciones             | [Ver](/03-funciones)       | declaración, parámetros, retorno    |
| 4   | Arrays                | [Ver](/04-arrays)          | `push`, `map`, `filter`            |
| 5   | Objetos               | [Ver](/05-objetos)         | propiedades, métodos, `this`       |
| 6   | DOM Básico            | [Ver](/06-dom)             | `querySelector`, `addEventListener`|
| ... | ...                   | ...                        | ...                                 |
| 30  | Proyecto Final        | [Ver](/30-proyecto)        | App To-Do con LocalStorage         |

---

## 🧩 Ejemplo Técnico (Día 1 - Variables)

```javascript
// Uso moderno (ES6+)
let nombre = "Ana"; // mutable
const EDAD = 28;    // inmutable

// Tipos primitivos
typeof "Hola";    // "string"
typeof 42;        // "number"
typeof true;      // "boolean"
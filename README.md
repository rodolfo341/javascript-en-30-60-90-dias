# 🧠 Guía Maestra de JavaScript (Básico, Intermedio, Avanzado)

*Documentación técnica inspirada en [MDN Web Docs](https://developer.mozilla.org/es/docs/Web/JavaScript), con ejemplos prácticos y especificaciones ECMAScript.*

---

## 📜 Tabla de Contenidos Técnica


### 🔵 **Nivel Básico** ([Ver Todos](./basico/README.md))
1. **[Sintaxis Básica](./basico/01-sintaxis/README.md)**  
   - Variables: `let`, `const`, `var` (hoisting)  
   - Tipos: primitivos vs objetos  
   - Operadores: `+`, `??`, `typeof`  

2. **[Estructuras de Control](/basico/02-control-flujo/README.md)**  
   - `if...else`, `switch`  
   - Bucles: `for`, `while`, `for...of`  

3. **[Funciones](/basico/03-funciones/README.md)**  
   - Declaración vs expresión  
   - Arrow functions (lexical `this`)  
   - Parámetros: default, rest  

4. **[Arrays](/basico/04-arrays/README.md)**  
   - Métodos: `map`, `filter`, `reduce`  
   - Spread operator (`...`)  

5. **[Objetos](/basico/05-objetos/README.md)**  
   - Notación literal vs `new Object()`  
   - Métodos estáticos: `Object.keys()`  

6. **[DOM Básico](/basico/06-dom/README.md)**  
   - `querySelector`, `addEventListener`  
   - Manipulación de clases (`classList`)  

7. **[ES6+ Essentials](/basico/07-es6/README.md)**  
   - Template literals  
   - Destructuring  

---

### 🟠 **Nivel Intermedio** ([Ver Todos](/intermedio/README.md))
1. **[Asincronía](/intermedio/01-asincronia/README.md)**  
   - Callback Hell → Promesas → Async/Await  
   - `Promise.allSettled()`  

2. **[POO Avanzada](/intermedio/02-poo/README.md)**  
   - Clases: herencia con `extends`  
   - Métodos privados (`#`)  

3. **[Módulos](/intermedio/03-modulos/README.md)**  
   - `import`/`export`  
   - Dynamic imports  

4. **[Gestión de Errores](/intermedio/04-errores/README.md)**  
   - Custom Errors (`class MiError extends Error`)  
   - Stack traces  

5. **[APIs Nativas](/intermedio/05-apis/README.md)**  
   - `fetch()`, `IntersectionObserver`  
   - `localStorage` vs `sessionStorage`  

6. **[Testing](/intermedio/06-testing/README.md)**  
   - Jest: `describe`, `expect`  
   - Mocking functions  

---

### 🔴 **Nivel Avanzado** ([Ver Todos](/avanzado/README.md))
1. **[Patrones de Diseño](/avanzado/01-patrones/README.md)**  
   - Singleton, Factory, Observer  

2. **[Performance](/avanzado/02-performance/README.md)**  
   - Debouncing vs Throttling  
   - Web Workers  

3. **[Seguridad](/avanzado/03-seguridad/README.md)**  
   - XSS, CSRF, CSP headers  

4. **[Tooling](/avanzado/04-tooling/README.md)**  
   - Webpack config básica  
   - Babel presets  

5. **[Frameworks](/avanzado/05-frameworks/README.md)**  
   - React Hooks vs Vue Composition API  

6. **[Node.js Básico](/avanzado/06-node/README.md)**  
   - Event Loop (fases)  
   - Streams  

---

## 🛠️ Ejemplo Técnico (Estilo MDN)

```javascript
// Ejemplo: Gestión de errores con async/await
async function fetchData(url) {
  try {
    const response = await fetch(url);
    if (!response.ok) throw new Error(`HTTP error! status: ${response.status}`);
    return await response.json();
  } catch (error) {
    console.error('Fetch failed:', error);
    throw error; // Re-throw para manejo externo
  }
}
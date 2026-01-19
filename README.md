# Comentarios del código HTML y CSS

## DOCTYPE y estructura básica
- **DOCTYPE:** Declaración que indica al navegador que este documento es HTML5  
- **Esta línea SIEMPRE debe ir al inicio de cualquier página web moderna**

- **Etiqueta HTML raíz:** Contiene TODO el contenido de la página  
- **lang="es":** Indica que el idioma del contenido es español (importante para accesibilidad y SEO)  
- **ALTERNATIVA:** lang="en" para inglés, lang="fr" para francés, etc.

---

## Sección HEAD
- **HEAD:** Sección de metadatos (información sobre la página que no se ve en pantalla)  
- Aquí van configuraciones, enlaces a CSS, JavaScript, fuentes, etc.

- **charset="UTF-8":** Define la codificación de caracteres (permite usar ñ, acentos, emojis, etc.)  
- **IMPORTANTE:** Siempre incluir esta línea para evitar problemas con caracteres especiales

- **viewport:** Hace que la página sea responsive (se adapte a móviles y tablets)  
- **width=device-width:** El ancho se ajusta al dispositivo  
- **initial-scale=1.0:** Zoom inicial al 100%  
- **EJERCICIO:** Prueba cambiar initial-scale=2.0 y observa cómo la página inicia con zoom

- **TITLE:** Texto que aparece en la pestaña del navegador  
- **EJERCICIO:** Cambia el título a "Mi Primera Calculadora Web" y observa la pestaña

---

## CSS – Estilos generales
- **SECCIÓN CSS:** Estilos visuales de la página  
- CSS define **CÓMO** se ven los elementos HTML (colores, tamaños, posiciones, etc.)

- **Selector universal (*):** Aplica estilos a TODOS los elementos HTML  
- Se usa para resetear estilos por defecto del navegador

- **margin:** Espacio EXTERIOR alrededor del elemento  
- **padding:** Espacio INTERIOR dentro del elemento  
- **DIFERENCIA:** margin empuja hacia afuera, padding hacia adentro

- **box-sizing:** Define cómo se calculan las dimensiones  
- **border-box:** Incluye padding y borde en width/height  
- **ALTERNATIVA:** content-box (menos intuitivo)

---

## Body y layout
- **BODY:** Contiene todo el contenido visible  
- **Flexbox:** Sistema moderno para centrar y crear layouts responsive  
- **justify-content + align-items:** Centrado perfecto  
- **100vh:** Altura completa de la ventana  
- **background:** Color de fondo hexadecimal  
- **position: relative:** Contexto para pseudo-elementos  
- **overflow: hidden:** Evita barras de desplazamiento

---

## Pseudo-elemento ::before
- **::before:** Crea contenido visual sin HTML extra  
- **content:** Obligatorio para que funcione  
- **position: absolute:** Sale del flujo normal  
- **width/height 200%:** Evita cortes al rotar  
- **radial-gradient:** Efectos de luz circular  
- **rgba:** Color con opacidad  
- **animation:** Animación continua de rotación

---

## Animaciones
- **@keyframes:** Define los pasos de una animación  
- **rotate:** Gira el fondo 360°  
- **pulse:** Efecto de pulsación (crecer + opacidad)

---

## Contenedor de la calculadora
- **Clase reutilizable (.calculadora)**  
- **rgba:** Fondo con transparencia  
- **backdrop-filter:** Efecto vidrio esmerilado  
- **border-radius:** Esquinas redondeadas  
- **box-shadow:** Sombras externas e internas  
- **width + max-width:** Diseño responsive controlado  
- **z-index:** Control de capas (profundidad)

---

## Títulos y texto
- **h1:** Encabezado principal (uno por página)  
- **text-align:** Alineación  
- **text-transform:** Mayúsculas  
- **letter-spacing:** Espaciado entre letras  
- **text-shadow:** Brillo en el texto  
- **font-weight:** Grosor de la fuente

---

## Campos de formulario
- **.campo:** Agrupa label + input  
- Facilita organización y estilos

- **label:** Mejora accesibilidad  
- **for + id:** Click en el label enfoca el input  
- **BUENA PRÁCTICA:** Siempre usar labels

---

## Inputs y selects
- **Selector múltiple:** Aplica estilos a varios elementos  
- **width: 100%:** Ocupan todo el ancho  
- **padding:** Área clickeable cómoda  
- **transition:** Cambios suaves  
- **:focus:** Estado cuando el usuario interactúa  
- **outline:** Se elimina solo si hay feedback visual alternativo

- **::placeholder:** Texto de ayuda sutil  
- No debe competir con el valor real

---

## Select personalizado
- **appearance: none:** Elimina estilo por defecto  
- **SVG embebido:** Flecha personalizada sin archivos externos  
- **background-position:** Control preciso de la flecha  
- **padding-right:** Evita solapamiento

---

## Campo de resultado
- Diferenciación visual clara  
- **Colores contrastantes:** Cyan vs rosa  
- **Texto grande y centrado:** Mayor énfasis  
- **Brillo exterior e interior:** Sensación de luz

---

## Icono decorativo
- Elemento puramente visual  
- Guía la atención del usuario  
- **Animación pulse:** Dinamismo  
- **drop-shadow:** Brillo que respeta la forma

---

## Body – Contenido visible
- Todo lo que se ve en pantalla va dentro del body

---

## Estructura HTML de la calculadora
- **DIV contenedor:** Agrupa toda la calculadora  
- **H1:** Título principal con emoji (UTF-8)  
- **EJERCICIO:** Cambiar emojis para variar diseño

- **Campos numéricos:**  
  - type="number": Solo números  
  - step="any": Permite decimales  
  - placeholder: Texto de ayuda  
  - id único para JavaScript y labels  

- **Select de operación:**  
  - Primera opción vacía como placeholder  
  - value es leído por JavaScript  
  - Texto es lo que ve el usuario  

- **BUENA PRÁCTICA GENERAL:**  
  - Código semántico  
  - Accesibilidad  
  - Diseño responsive  
  - Comentarios claros para aprendizaje
# Calculadora_conmd

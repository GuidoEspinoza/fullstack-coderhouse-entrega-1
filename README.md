# Mi Sitio Web - Pre-entrega

## 📋 Descripción del Proyecto

Este es un sitio web desarrollado como pre-entrega del curso de Full Stack de CoderHouse. El proyecto implementa una estructura completa de sitio web utilizando HTML5, **SCSS**, Bootstrap 5 y animaciones CSS, con un enfoque en diseño responsivo, arquitectura modular y mejores prácticas de desarrollo web.

## 🚀 Características Principales

### ✅ Estructura Completa
- **Páginas HTML** con contenido completo y maquetado profesional
- **Navegación consistente** en todas las páginas
- **Diseño responsivo** optimizado para desktop y mobile
- **Arquitectura SCSS modular** con partials organizados

### ✅ Tecnologías Utilizadas
- **HTML5** - Estructura semántica y accesible
- **SCSS** - Preprocesador CSS con variables, mixins y nesting
- **CSS3** - Animaciones y transiciones avanzadas
- **Bootstrap 5** - Framework CSS para componentes y grid system
- **Metodología BEM** - Nomenclatura de clases CSS
- **Sass** - Compilación y watch mode para desarrollo

### ✅ Componentes de Bootstrap Implementados
1. **Navbar Responsiva** - Navegación con collapse y menú hamburguesa
2. **Carousel** - Carrusel de características con indicadores y controles
3. **Cards** - Sistema de tarjetas para habilidades con altura uniforme
4. **Forms** - Formularios con validación y grid responsive
5. **Grid System** - Layout responsivo con breakpoints múltiples
6. **Modal (CSS)** - Sistema de confirmación sin JavaScript
7. **Buttons** - Botones estilizados con diferentes variantes
8. **Responsive Utilities** - Clases para diferentes dispositivos

### ✅ Características SCSS Avanzadas
- **Variables globales** para colores, tipografía y espaciado
- **Mixins reutilizables** para responsive design y componentes
- **Nesting estructurado** siguiendo metodología BEM
- **Partials organizados** por funcionalidad
- **Extends/placeholders** para código DRY
- **Animaciones keyframes** para interactividad

## 📁 Estructura del Proyecto

```
pre-entrega/
├── index.html                    # Página principal con carrusel Bootstrap
├── styles.css                    # CSS compilado desde SCSS
├── styles.css.map                # Source map para debugging
├── README.md                     # Documentación completa del proyecto
├── pages/
│   ├── about.html                # Página "Acerca de" con cards y video
│   └── contact.html              # Página de contacto con modal CSS
├── scss/                         # Arquitectura SCSS modular
│   ├── styles.scss               # Archivo principal SCSS
│   ├── _variables.scss           # Variables globales (colores, tipografía, etc.)
│   ├── _mixins.scss              # Mixins y extends reutilizables
│   ├── _base.scss                # Reset, tipografía base y contenedores
│   ├── _components.scss          # Componentes específicos (hero, cards, etc.)
│   ├── _animations.scss          # Keyframes y animaciones CSS
│   └── _responsive.scss          # Media queries y responsive design
└── assets/                       # Recursos del proyecto
    ├── desarrollo-web.jpg        # Imagen para el artículo destacado
    └── profile_image_new.jpeg    # Foto de perfil para página About
```

## 🎯 Páginas del Sitio

### 1. **Inicio** (`index.html`)
- Hero section responsive con imagen centrada
- Carrusel de Bootstrap con 3 características principales
- Artículo destacado con diseño visual atractivo
- Navegación adaptativa con menú hamburguesa
- **Animaciones**: Fade in, slide in y efectos hover

### 2. **Acerca de** (`pages/about.html`)
- Presentación personal con foto de perfil responsiva
- Grid de habilidades con 3 cards Bootstrap (Frontend, Backend, Herramientas)
- Video de presentación embedded de YouTube con ratio 16:9
- Diseño completamente adaptativo para todos los dispositivos
- **Animaciones**: Cards con efectos hover y transiciones suaves

### 3. **Contacto** (`pages/contact.html`)
- Formulario responsivo con validación HTML5
- Layout en 2 columnas (desktop) / 1 columna (mobile)
- Información de contacto con iconos visuales
- Modal de confirmación implementado solo con CSS (sin JavaScript)
- **Animaciones**: Transiciones de formulario y modal

## 🛠️ Funcionalidades Especiales

### 🎯 **Modal CSS Puro (Sin JavaScript)**
El formulario de contacto implementa una solución innovadora de modal:
- **Tecnología**: CSS `:target` selector + HTML anchor links
- **Activación**: Al enviar formulario (`action="#success"`)
- **Características**: Overlay translúcido, centrado responsive, botones de acción
- **Ventajas**: Cero dependencias JavaScript, funcionamiento universal
- **UX**: Transiciones suaves y experiencia completa

### 🎠 **Carrusel Bootstrap Avanzado**
- **3 slides informativos** con iconos emoji y descripciones
- **Controles responsive**: Flechas grandes (desktop) / pequeñas circulares (mobile)
- **Indicadores de posición** para navegación directa
- **Auto-slide** activado con controles manuales disponibles
- **Optimización móvil**: Controles reposicionados y redimensionados

### 🧭 **Navegación Adaptativa**
- **Menú hamburguesa** en resoluciones móviles
- **Links activos** con estados visuales según página actual
- **Logo consistente** con tipografía responsive
- **Transiciones Bootstrap** integradas naturalmente

### 🎨 **Sistema de Animaciones CSS**
- **Keyframes personalizados**: fadeIn, slideInLeft, bounce, pulse, rotate, shake
- **Clases de animación**: `.animate-fade-in`, `.animate-slide-in`, etc.
- **Delays escalonados**: `.animation-delay-1`, `.animation-delay-2`, etc.
- **Efectos hover**: Transiciones suaves en botones y cards
- **Performance optimizada**: Uso de `transform` y `opacity`

## 📱 Responsive Design

### 🖥️ **Desktop (1200px+)**
- Layout de 2-3 columnas optimizado
- Carrusel con flechas de navegación visibles
- Formulario en 2 columnas (Nombre/Email)
- Video con altura completa
- Navegación horizontal extendida
- Animaciones completas activadas

### 📟 **Tablet (769px - 1024px)**
- Adaptación intermedia de componentes
- Video con altura media (300px)
- Cards reorganizadas según espacio disponible
- Imagen de perfil de tamaño intermedio (250px)
- Animaciones optimizadas para touch

### 📱 **Mobile (<768px)**
- Layout de 1 columna optimizado
- Carrusel con controles circulares más pequeños
- Formulario completamente apilado
- Video responsivo con altura reducida (200px)
- Navegación colapsible con menú hamburguesa
- Tipografía ajustada para legibilidad móvil
- Imagen de perfil reducida para móviles (200px)
- Animaciones simplificadas para mejor performance

## 🎨 Arquitectura SCSS

### 📋 **Variables Globales** (`_variables.scss`)
```scss
// Colores principales
$primary-color: #007bff;
$secondary-color: #6c757d;
$success-color: #28a745;
$danger-color: #dc3545;

// Tipografía
$font-family-base: 'Arial', sans-serif;
$font-size-base: 1rem;
$line-height-base: 1.5;

// Espaciado
$spacing-xs: 0.25rem;
$spacing-sm: 0.5rem;
$spacing-md: 1rem;
$spacing-lg: 1.5rem;
$spacing-xl: 3rem;

// Breakpoints
$mobile-max: 768px;
$tablet-max: 1024px;
$desktop-min: 1200px;
```

### 🔧 **Mixins Reutilizables** (`_mixins.scss`)
```scss
// Responsive design
@mixin mobile-up { @media (max-width: $mobile-max) { @content; } }
@mixin tablet { @media (min-width: #{$mobile-max + 1px}) and (max-width: $tablet-max) { @content; } }
@mixin desktop { @media (min-width: $desktop-min) { @content; } }

// Componentes
@mixin container-base {
  max-width: $container-max-width;
  margin: 0 auto;
  padding: 0 0.75rem;
  width: 100%;
}

@mixin center-flex {
  display: flex;
  justify-content: center;
  align-items: center;
}

@mixin smooth-transition($property: all, $duration: 0.3s) {
  transition: $property $duration ease-in-out;
}
```

### 🎭 **Extends/Placeholders** (`_mixins.scss`)
```scss
// Texto muted
%text-muted {
  color: $muted-color;
}

// Botones base
%button-base {
  border: none;
  border-radius: $border-radius;
  padding: $spacing-sm $spacing-md;
  @include smooth-transition();
  cursor: pointer;
}
```

## 🚦 Desarrollo con SCSS

### Compilación Manual
```bash
# Compilar una vez
sass scss/styles.scss styles.css

# Compilar con source maps
sass --source-map scss/styles.scss styles.css
```

### Modo Watch (Recomendado)
```bash
# Watch mode con source maps
sass --watch scss/styles.scss styles.css

# El comando monitorea cambios y recompila automáticamente
```

### Estructura de Importación
```scss
// styles.scss - Archivo principal
@use 'sass:color';
@forward 'variables';
@forward 'mixins';
@use 'variables' as *;
@use 'mixins' as *;
@use 'base';
@use 'components';
@use 'animations';
@use 'responsive';
```

## 🎨 Metodología BEM

El proyecto utiliza la metodología BEM (Block Element Modifier) para la nomenclatura de clases:

```scss
/* Ejemplo de estructura BEM en SCSS */
.header {                    // Block
  &__logo {                 // Element
    font-size: 1.5rem;
  }
  
  &__nav {                  // Element
    display: flex;
  }
  
  &__link {                 // Element
    text-decoration: none;
    
    &--active {             // Modifier
      font-weight: bold;
      color: $primary-color;
    }
  }
}
```

## 🔬 Innovaciones Técnicas Implementadas

### 🎯 **Modal CSS Puro - Zero JavaScript**
```scss
.modal-overlay {
  display: none;
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.5);
  z-index: 1000;
  
  &:target {
    display: flex;
    justify-content: center;
    align-items: center;
  }
}
```

### 📱 **Responsive Carousel Controls**
```scss
.carousel-control-prev,
.carousel-control-next {
  @include mobile-up {
    width: 40px;
    height: 40px;
    border-radius: 50%;
    background-color: rgba(0, 0, 0, 0.3);
  }
}
```

### 🎨 **Smart Typography Scaling**
```scss
.hero {
  &__title {
    font-size: 3rem;
    
    @include mobile-up {
      font-size: 2rem;
    }
  }
  
  &__subtitle {
    font-size: 1.25rem;
    
    @include mobile-up {
      font-size: 1.1rem;
    }
  }
}
```

### 🎭 **Sistema de Animaciones Modular**
```scss
// Keyframes base
@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}

@keyframes slideInLeft {
  from {
    opacity: 0;
    transform: translateX(-30px);
  }
  to {
    opacity: 1;
    transform: translateX(0);
  }
}

// Clases de animación
.animate-fade-in {
  animation: fadeIn 0.6s ease-out;
}

.animate-slide-in {
  animation: slideInLeft 0.8s ease-out;
}

// Delays escalonados
@for $i from 1 through 5 {
  .animation-delay-#{$i} {
    animation-delay: #{$i * 0.1}s;
  }
}
```

## 🌟 Características Adicionales Implementadas

### 🎨 **Diseño Visual**
- **Paleta de colores consistente** definida en variables SCSS
- **Iconos emoji** para compatibilidad universal sin dependencias
- **Sombras y efectos** de Bootstrap + customizaciones SCSS
- **Tipografía escalable** con sistema de variables
- **Animaciones fluidas** con keyframes personalizados

### 🔧 **Optimizaciones Técnicas**
- **SCSS modular**: Arquitectura escalable con partials
- **Variables centralizadas**: Fácil mantenimiento y consistencia
- **Mixins reutilizables**: Código DRY y eficiente
- **Media queries organizadas**: Responsive design estructurado
- **Source maps**: Debugging fácil en desarrollo
- **Watch mode**: Compilación automática en desarrollo

### 📊 **Performance y UX**
- **CSS optimizado**: Compilación eficiente desde SCSS
- **Animaciones performantes**: Uso de `transform` y `opacity`
- **Carga rápida**: Assets optimizados y CDN
- **Navegación intuitiva**: Estados activos y transiciones naturales
- **Accesibilidad**: Labels, alt texts, y aria attributes
- **Cross-browser**: Compatible con navegadores modernos

### 🛠️ **Herramientas de Desarrollo**
- **Metodología BEM**: Nomenclatura clara y mantenible
- **Arquitectura SCSS**: Estructura modular y escalable
- **Sass compilation**: Workflow de desarrollo optimizado
- **Source maps**: Debugging eficiente
- **Documentación completa**: README detallado con ejemplos
- **Git workflow**: Historial limpio con commits semánticos

## 📝 Notas de Desarrollo

### Decisiones de Arquitectura SCSS
- **Partials organizados**: Separación por funcionalidad
- **Variables centralizadas**: Mantenimiento simplificado
- **Mixins estratégicos**: Reutilización de código común
- **Nesting controlado**: Máximo 3 niveles de profundidad
- **BEM + SCSS**: Nomenclatura clara con nesting estructurado

### Optimizaciones de Performance
- **CSS compilado optimizado**: Eliminación de código redundante
- **Animaciones eficientes**: Uso de propiedades que no causan reflow
- **Media queries consolidadas**: Agrupación inteligente de breakpoints
- **Source maps en desarrollo**: Debugging sin impacto en producción
- **Watch mode**: Desarrollo ágil con recompilación automática

### Decisiones de UX/UI
- **Mobile-first approach**: Diseño desde móvil hacia desktop
- **Progressive enhancement**: Funcionalidad básica + mejoras por capas
- **Animaciones sutiles**: Mejora de UX sin distracciones
- **Consistencia visual**: Variables SCSS para coherencia
- **Responsive animations**: Adaptación de animaciones por dispositivo

## 📊 Cumplimiento de Requisitos

### ✅ Estructura Avanzada
- [x] Todos los HTML con contenido suficiente
- [x] Maquetado para vista desktop
- [x] Uso de Flexbox, Grid y Bootstrap
- [x] **Migración completa a SCSS**
- [x] **Arquitectura modular con partials**

### ✅ Responsive Design
- [x] **Todas las páginas** adaptadas a móvil con breakpoints específicos
- [x] **3 rangos de dispositivos**: Mobile (<768px), Tablet (769-1024px), Desktop (1200px+)
- [x] **Layouts diferenciados** por dispositivo (no solo centrado)
- [x] **Componentes adaptativos**: Carrusel, formularios, navegación, cards
- [x] **Tipografía escalable** con variables SCSS
- [x] **Imágenes responsivas** con tamaños optimizados

### ✅ Componentes Bootstrap
- [x] **8+ componentes** implementados (Navbar, Carousel, Cards, Forms, Grid, Modal, Buttons, Utils)
- [x] **Sistema de grillas completo** para responsive design
- [x] **Combinación inteligente** de componentes y grillas personalizadas
- [x] **Bootstrap usado estratégicamente** (no para maquetado básico)
- [x] **Customización con SCSS** para estilos específicos

### ✅ Características SCSS Avanzadas
- [x] **Variables globales** para colores, tipografía y espaciado
- [x] **Mixins reutilizables** para responsive y componentes
- [x] **Nesting estructurado** siguiendo BEM
- [x] **Partials organizados** por funcionalidad
- [x] **Extends/placeholders** para código DRY
- [x] **Animaciones keyframes** modulares
- [x] **Compilación optimizada** con source maps

## 👨‍💻 Autor

**Guido Espinoza**
- Estudiante de Full Stack - CoderHouse
- GitHub: [@GuidoEspinoza](https://github.com/GuidoEspinoza)
- Email: contacto@guidoespinoza.dev

## 📊 Estadísticas del Proyecto

- **📄 Páginas**: 3 páginas principales completamente funcionales
- **💻 Líneas de código**: ~450 líneas HTML + ~300 líneas SCSS
- **🎨 Componentes Bootstrap**: 8+ componentes implementados
- **📱 Breakpoints**: 3 rangos responsivos (Mobile, Tablet, Desktop)
- **🎭 Animaciones**: 6 keyframes + clases de animación
- **⚡ Performance**: <2s carga completa con Bootstrap CDN
- **🔧 Dependencias**: Bootstrap 5 (CDN) + Sass (desarrollo)
- **📝 Metodología**: BEM + SCSS + Mobile-first + Progressive enhancement
- **📁 Arquitectura**: 7 archivos SCSS modulares

## 📄 Licencia

Este proyecto es parte de un curso educativo y está disponible para fines de aprendizaje.

---

*Desarrollado con ❤️ como parte del curso Full Stack de CoderHouse - Enero 2025*
*Migrado a SCSS con arquitectura modular y sistema de animaciones avanzado*

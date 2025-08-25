# Cancheros Ind

# Migración a SASS y Mejoras de Estructura

Este proyecto ha sido migrado a SASS y mejorado con las siguientes características:

# Estructura de Carpetas

```
scss/
├── base/
│   ├── _vars.scss         # Variables globales
│   ├── _mixins.scss       # Mixins reutilizables
│   └── _animaciones.scss  # Animaciones y keyframes
├── components/
│   ├── _navbar.scss       # Estilos del navbar
│   └── _footer.scss       # Estilos del footer
├── layouts/
│   ├── _index.scss        # Estilos página principal
│   ├── _productos.scss    # Estilos sección productos
│   ├── _marcas.scss       # Estilos sección marcas
│   └── _quienes_somos.scss
└── index.scss             # Archivo principal de importación
```

# Características SASS Implementadas

# Variables

```scss
// Colores principales
$colorPrimario: #c02924;
$colorSecundario: #203580;
$colorTercero: #ffffff;

// Tipografía
$fuentePrincipal: "Nunito", sans-serif;
$fontSize-base: 1rem;
```

# Mixins

```scss
// Mixin para botones
@mixin boton($bg-color, $text-color, $size) {
  background-color: $bg-color;
  color: $text-color;
  // ...más estilos
}

// Mixin para cards
@mixin card($padding: $spacing-md, $shadow: true) {
  background: $colorTercero;
  border-radius: $border-radius-lg;
  // ...más estilos
}
```

Anidaciones y BEM

```scss
.productos {
  &__header {
    // Estilos del header
  }

  &__grid {
    // Sistema de grid personalizado
  }

  &__card {
    // Estilos de cards
  }
}
```

- `fadeIn`: Aparición suave
- `slideUp`: Deslizamiento hacia arriba
- `pulse`: Efecto de latido
- `bounce`: Efecto de rebote

- Uso de clases utilitarias de Bootstrap
- Sistema de grid responsive
- Componentes personalizados con Bootstrap

- Eliminación de enlaces duplicados
- Orden correcto de carga (Bootstrap y Custom SCSS)

. **Responsive Design**

- Media queries personalizados
- Uso de variables para breakpoints
- Adaptación a diferentes dispositivos

# Características que agregué para esta entrega

- Sistema de diseño consistente con variables SASS
- Componentes reutilizables con mixins
- Animaciones personalizadas
- Grid system híbrido (Bootstrap + CSS Grid)
- Nomenclatura BEM para mejor mantenibilidad
- Correción estilos en pages/sale.html

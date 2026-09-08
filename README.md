# YDOM Support for VS Code

Este es el soporte de lenguaje oficial para **YDOM** (YAML DOM), el moderno framework de UI reactiva y declarativa basado en indentación. 

Añade reglas personalizadas de sintaxis y autocompletado avanzado que no están presentes en YAML ni HTML nativo, brindando una experiencia de desarrollo (*Developer Experience*) de primer nivel.

## ✨ Características Principales

- 🌳 **Resaltado Jerárquico Impecable**: Reconocimiento de etiquetas (tags) basándose en la estricta indentación de YDOM.
- ⚙️ **Control Flow Avanzado**: Resaltado brillante y estructurado para directivas de flujo como `@if`, `@else-if`, `@else` y bucles `@for (item) in items`.
- 🎨 **Atributos y Propiedades**: Soporte dedicado para el bloque de atributos entre paréntesis `(class="card")`.
- ⚡ **Eventos y Data Binding**: Colores semánticos para eventos nativos (`@click`, `@submit`) y binding de propiedades reactivas (`:value`, `:class`).
- 🧠 **Interpolación Inteligente (`{{ }}`)**: La sintaxis de interpolación comprende variables locales, cadenas, booleanos y ejecución de métodos inofensivos (`{{ names.join(', ') }}`).
- 📝 **Comentarios de Código**: Soporte nativo para comentarios de una sola línea con `//`, idéntico a JS/TS y completamente invisibles en el DOM final.
- 🧩 **Pares Ágiles**: Autocierre rápido para paréntesis `()`, corchetes, comillas `""` y backticks ` `` `.

## 🚀 Sintaxis de Ejemplo

```ydom
div
  // Encabezado principal
  h1: YDOM App

  div
    (class="card" :style="dynamicStyle")
    
    @if user.isLogged
      p: Bienvenido, {{ user.name.toUpperCase() }}
      button: Cerrar Sesión
        (@click="logout()")
        
    @else
      p: Por favor, inicia sesión.

    // Iteración de elementos
    ul
      @for (item, index) in items
        li: {{ index }} - {{ item.title }}
```

## 🛠 Instalación y Empaquetado

Para compilar la extensión y subirla a la tienda de **VS Code** o **Antigravity Store**:

```bash
# 1. Instalar dependencias globalmente
npm install -g @vscode/vsce

# 2. Empaquetar la extensión (.vsix)
npm run build
```

Una vez generado el archivo `ydom-vscode-x.x.x.vsix`, puedes subirlo al Marketplace de Visual Studio Code o instalarlo localmente en tu editor.

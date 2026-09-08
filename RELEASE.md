# YDOM for VS Code - v1.1.0 🚀

## Resumen

La nueva actualización oficial de soporte estructurado para **YDOM (YAML DOM)** ya está lista para su despliegue en el VS Code Marketplace. Hemos ampliado enormemente la gramática para dar soporte a las nuevas especificaciones de renderizado, interpolación y estructuras de control.

## 🌟 Novedades en esta versión

- 🔄 **Soporte para Control Flow**: Añadido resaltado de sintaxis preciso para `@if`, `@else-if`, `@else` y `@for`. 
- 💬 **Comentarios JS-Style (`//`)**: Se ha implementado el soporte oficial para los comentarios con doble barra, haciendo que el código sea limpio y consistente con TypeScript.
- 🧠 **Interpolación Enriquecida (`{{ }}`)**: El resaltado de sintaxis dentro de las llaves ahora comprende encadenamientos de métodos (`.join()`), variables, booleanos (`true`/`false`) y números.
- 📦 **Bloque de Atributos (`()`)**: Mejora en el reconocimiento del bloque de atributos encapsulado en paréntesis directamente debajo de un tag, permitiendo un coloreado semántico perfecto para propiedades nativas.
- 🎉 **Lanzamiento de Soporte Nativo**: Implementación pura de gramática usando JSON TextMate.
- ⚡ **Eventos (YDOM Specs)**: Resaltado agresivo brillante para los comandos de inyección lógica como eventos nativos (`@click`).
- 🔗 **Data Binding Sensible**: Parseo de inyección de propiedades tipo prop-drilling (`:value`).
- 🧩 **Pares Ágiles**: Auto-matching rápido y cerrado para paréntesis estructurales `()`, comillas dobles y backticks de contenido dinámico.

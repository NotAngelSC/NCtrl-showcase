# Guía para completar el showcase

Este repositorio contiene solo material público del portafolio. El código y la documentación técnica de NCtrl permanecen en otro repositorio privado.

## Completar la presentación

Edita `README.md` y sustituye los comentarios de «Pendiente» por secciones breves, en este orden:

1. Descripción del proyecto y problema que atiende.
2. Funciones seleccionadas y verificadas, con el alcance real de cada una.
3. Tu participación: qué hiciste, qué decisiones tomaste y qué trabajo fue compartido.
4. Tecnologías generales, sin copiar configuraciones ni contratos internos.
5. Capturas revisadas.
6. Enlace al video de demostración alojado externamente.
7. Estado real del proyecto y una forma de contacto que decidas publicar.

Documenta resultados solo si tienes evidencia y explica el contexto de su medición. Evita atribuirte trabajo de otras personas. Decide por separado si quieres añadir una licencia para los materiales públicos; por ahora no hay licencia de reutilización.

## Imágenes y video

Guarda las capturas en `assets/capturas/` y una portada opcional en `assets/portada/`. Usa nombres descriptivos en minúsculas, sin espacios ni datos personales, por ejemplo `panel-principal-01.webp`. Exporta con el ancho necesario para lectura y comprime antes de añadir; WebP o PNG son adecuados para interfaz. Mantén un tamaño razonable para Git y elimina metadatos cuando corresponda.

Inserta imágenes con rutas relativas desde el README, por ejemplo:

```markdown
![Vista del panel con datos ficticios](assets/capturas/panel-principal-01.webp)
```

Añade la línea solo cuando exista el archivo. Para el video, publica en un servicio externo elegido por ti y añade un enlace Markdown a la URL real. No subas videos grandes a Git.

Usa únicamente datos ficticios. Antes de publicar cada captura o video, revisa nombres, correos, folios, fechas, archivos adjuntos, pestañas, notificaciones y metadatos visibles. Confirma que no aparezcan personas, clientes o empresas reales ni credenciales.

## Actualizar solo este repositorio

Ejecuta los comandos con la ruta explícita para evitar cambios en el proyecto privado:

```bash
git -C /home/angel/proyectos/NCtrl-showcase status --short
git -C /home/angel/proyectos/NCtrl-showcase add README.md GUIA_ACTUALIZACION.md assets/capturas assets/portada
git -C /home/angel/proyectos/NCtrl-showcase diff --cached --stat
git -C /home/angel/proyectos/NCtrl-showcase commit -m "Completar material público de NCtrl"
git -C /home/angel/proyectos/NCtrl-showcase push origin main
```

Cuando el contenido esté listo, abre tu perfil de GitHub, entra en **Customize your pins** y selecciona `NCtrl-showcase`. GitHub Pages y cualquier demo desplegada quedan para una fase posterior.

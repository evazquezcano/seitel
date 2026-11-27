# SEITEL 2.0 — versión de pruebas

Rama `seitel-v2-pruebas`. No desplegada en la web pública.

## Probar
Descargar el ZIP de la rama, descomprimir todos los archivos y abrir `index.html` con Chrome o Edge. Los bancos y los logotipos se cargan localmente. El acceso a pretest/postest en la prueba local remite a la web original (requiere conexión). En GitHub Pages, `legacy.html` conserva el código original y el banco `questions.json` para esas modalidades.

## Archivos
- `index.html`: interfaz, configuración por asignatura y motor de autoevaluación.
- `bancos/ecp.js`: 279 preguntas activas de Evaluación de Centros y Profesores; tres opciones y explicaciones por distractor.
- `bancos/mrdte.js`: copia íntegra del banco original, sin modificar sus claves.
- `legacy.html` y `questions.json`: versión anterior, conservada.

## Validación
ECP: 15 ítems por simulacro, cuotas 2/2/2/2/2/1/2/1/1, +0,4/−0,2/0. Prácticas de 10. Se corrigió la etiqueta del distractor del tema 1, pregunta 24; se excluyó provisionalmente la pregunta 3 del tema 6 por contradicción en el enunciado. No se han modificado las respuestas correctas del banco original. La interfaz nueva excluye provisionalmente el ítem 32 de Exámenes pasadas convocatorias de MRDyTE (opciones mezcladas con el siguiente enunciado), pero lo conserva intacto en los ficheros originales. Se conserva el orden de alternativas de MRDyTE. La nueva interfaz no transmite eventos analíticos durante las pruebas; el acceso a la versión antigua conserva su configuración original.

No integrar en main hasta completar la validación docente.

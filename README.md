# Tú – Consultorio Empresarial | Prototipo GitHub Pages sin costo de API

## Publicación gratuita

1. Crea una cuenta en https://github.com si todavía no tienes.
2. En GitHub, selecciona **New repository** y asígnale el nombre `tu-consultorio-cargos`.
3. Selecciona **Public**. GitHub Pages de GitHub Free requiere un repositorio público. No subas respuestas reales ni datos de clientes al repositorio.
4. En **Add file → Upload files**, sube `index.html` y `.nojekyll` (este último es opcional), y confirma con **Commit changes**.
5. Ve a **Settings → Pages → Build and deployment → Deploy from a branch**, elige `main` y `/ (root)`, y guarda.
6. Abre la dirección mostrada por GitHub, que tendrá la forma `https://TU-USUARIO.github.io/tu-consultorio-cargos/`.

## Cómo funciona

- No requiere Python, servidor, API key ni tarjeta bancaria.
- La interpretación se intenta ejecutar dentro del navegador usando WebLLM y el modelo `Qwen3-1.7B-q4f16_1-MLC`.
- La primera ejecución descarga un modelo grande desde el proveedor de archivos, usando Internet y almacenamiento local.
- Requiere WebGPU compatible y recursos suficientes; Chrome/Edge reciente con aceleración por hardware suele ser la opción más adecuada.
- Los relatos no se envían a una API de pago. El navegador descarga código y los archivos del modelo de servidores externos.
- El contenido generado puede ser impreciso: verificar el informe con la empresaria antes de usarlo formalmente.
- El botón de Word genera un HTML con extensión `.doc` para abrir en Word, no un DOCX nativo.
- **El paquete está preparado pero la inferencia no se ha probado en un equipo Windows con WebGPU desde este entorno.** Puede requerir cambios de compatibilidad. No se garantiza precisión de un modelo pequeño de 1,7B parámetros.

## Limitaciones importantes

GitHub Pages no ejecuta `server.py` ni ofrece inferencia de IA. Por eso esta versión prescinde del servidor y usa un motor local del navegador. GitHub no recibe automáticamente las respuestas, ni podrás acceder a los informes de los clientes sin que te los compartan. Para confidencialidad, no coloques testimonios, informes o datos de clientes dentro del repositorio público. Verifica licencias, condiciones y privacidad de dependencias externas antes de un lanzamiento abierto.

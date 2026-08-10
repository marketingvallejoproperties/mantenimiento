# Centro de Operaciones de Mantenimiento

Aplicación estática para Vallejo Properties construida con HTML, CSS y
JavaScript, conectada al proyecto Supabase **Mantenimiento**.

## Uso

1. Abra `index.html` desde un servidor estático o GitHub Pages. La información
   puede consultarse directamente, sin iniciar sesión.
2. Para cargar una nueva base, pulse **Acceso para cargar**. En el primer uso,
   escriba una contraseña de al
   menos ocho caracteres y pulse **Crear primer acceso**. Si Supabase solicita
   confirmación, revise el correo autorizado y después regrese para iniciar
   sesión.
3. Use **Cargar Excel** para seleccionar una versión actualizada de
   `Centro de Operaciones.xlsx`.
4. Los filtros, indicadores, alertas, gráficas y tablas se recalculan y la
   nueva base queda disponible para los usuarios autorizados.

La carpeta completa puede publicarse directamente en GitHub Pages. El archivo
`data/default-data.js` conserva una copia inicial para que el dashboard también
pueda abrirse sin conexión. La versión compartida se guarda en Supabase y
reemplaza la base anterior cada vez que se carga un Excel válido.

El correo inicialmente autorizado para cargar información es
`mariapropierties@gmail.com`. Otros usuarios pueden visualizar el dashboard con
el enlace, pero no pueden reemplazar la base. La clave
incluida en `supabase-config.js` es publicable; los permisos reales están
protegidos en la base mediante inicio de sesión y políticas de acceso.

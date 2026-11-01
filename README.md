# CARE · Examen Médico Laboral

Aplicación instalable en celulares y tabletas (Android y iOS) para realizar el examen médico laboral dirigido de **Seguridad Industrial CARE S. de R.L. de C.V.**, con base en el formato SHI-FOR-41.

Este repositorio solo contiene el programa. **Ningún dato de pacientes se sube a GitHub**: los expedientes se guardan únicamente en la memoria de cada dispositivo.

---

## Parte 1. Publicar la aplicación en GitHub (una sola vez)

No necesita instalar programas; todo se hace desde el navegador de una computadora.

1. Entre a **github.com** y cree una cuenta gratuita (o inicie sesión).
2. Arriba a la derecha, toque **+** → **New repository** (Nuevo repositorio).
3. Llene los datos:
   - **Repository name:** `examen-medico`
   - Seleccione **Public** (GitHub Pages gratuito requiere repositorio público; el programa no contiene datos personales).
   - Presione **Create repository**.
4. En la pantalla del repositorio nuevo, haga clic en **uploading an existing file** (subir un archivo existente).
5. Descomprima el archivo `CARE-Examen-Medico-GitHub.zip` en su computadora y **arrastre todos los archivos** a la página de GitHub:
   `index.html`, `manifest.webmanifest`, `sw.js`, `icon-192.png`, `icon-512.png`, `.nojekyll` y `README.md`.
   > Si no ve el archivo `.nojekyll` (está oculto), en Windows active *Vista → Elementos ocultos*; en Mac presione `Cmd + Shift + .`
6. Abajo, presione **Commit changes** (Guardar cambios).
7. Vaya a **Settings** (Configuración) → menú izquierdo **Pages**.
8. En **Build and deployment**:
   - **Source:** *Deploy from a branch*
   - **Branch:** `main` y carpeta `/ (root)`
   - Presione **Save**.
9. Espere de 1 a 3 minutos y recargue la página. Aparecerá la dirección de la aplicación:

   **`https://SU-USUARIO.github.io/examen-medico/`**

   Esa es la dirección que se abrirá en los dispositivos.

---

## Parte 2. Instalar la aplicación en cada dispositivo

### Android (Chrome)
1. Abra **Chrome** y escriba la dirección `https://SU-USUARIO.github.io/examen-medico/`.
2. Toque el menú **⋮** (arriba a la derecha) → **Instalar aplicación** o **Agregar a la pantalla principal**.
3. Confirme con **Instalar**. Aparecerá el ícono de CARE en su pantalla.

### iPhone y iPad (Safari)
1. Abra **Safari** (debe ser Safari) y escriba la dirección.
2. Toque el botón **Compartir** (cuadro con flecha hacia arriba).
3. Deslice y toque **Agregar a pantalla de inicio** → **Agregar**.

### Primer uso
- Abra la app **una vez con internet**; a partir de ahí funciona **sin conexión**.
- Si el navegador pregunta por permiso de almacenamiento, acéptelo: así los expedientes no se borran solos.
- Folio: **CARE-ACRÓNIMO-MES-CONSECUTIVO** (ejemplo: CARE-TMAL-11-001). El acrónimo (2 a 6 letras) identifica el proyecto, oficina o empresa; el consecutivo es **único por dispositivo** y reinicia en 001 cada mes, sin importar el acrónimo.

---

## Parte 3. Operación diaria

1. **Nuevo examen** → tipo (Ingreso, Periódico o Egreso), empresa, proyecto, **acrónimo** y lugar de trabajo.
2. Capture los datos del trabajador y el **perfil de riesgo del puesto**; con eso se activan las preguntas dirigidas.
3. Avance sección por sección. El **Agente clínico CARE** analiza cada respuesta y propone un dictamen.
4. En *Estudios complementarios*, para el antidoping elija el panel (1, 3 o 5 elementos), marque los reactivos y registre Negativo o Positivo en cada uno.
5. En *Análisis y dictamen*, avale o modifique la recomendación, y firmen evaluador y trabajador.
6. **Finalizar** asigna el folio y bloquea el expediente.
7. **Enviar expediente Word** abre el menú del teléfono para mandarlo por correo, WhatsApp o mensajería. **Constancia para la empresa** solo incluye aptitud y restricciones.
8. **Imprima el expediente y archívelo.** El expediente impreso se conserva **5 años** (NOM-004-SSA3-2012).

### Cierre de mes
Al abrir la app el primer día de un mes nuevo aparece el **Cierre de mes**:
1. **Compartir todos los Word** y **Descargar respaldo (.json)**.
2. Confirme que los expedientes están impresos y archivados.
3. **Depurar**: se borran del dispositivo y la numeración vuelve a 001.

---

## Parte 4. Actualizar a una nueva versión

1. En GitHub, abra el repositorio → **Add file** → **Upload files**.
2. Arrastre el nuevo `index.html` (y `sw.js` si viene incluido) → **Commit changes**.
3. En cada dispositivo, abra la app con internet, **ciérrela y vuelva a abrirla**. Tomará la versión nueva.

Los expedientes guardados en el dispositivo **no se pierden** al actualizar.

## Control de cambios
La aplicación no admite modificaciones. Cualquier cambio al cuestionario, a los criterios o al formato se solicita escribiendo la instrucción seguida de la frase de autorización de soporte. Dentro de la app, el acceso de soporte (Historial → Soporte) funciona igual y queda registrado en bitácora.

## Problemas frecuentes
| Situación | Solución |
|---|---|
| La dirección muestra error 404 | Espere 3 minutos después de activar Pages y verifique que `index.html` esté en la raíz del repositorio. |
| No aparece “Instalar aplicación” | Use Chrome en Android o Safari en iPhone; la dirección debe empezar con `https://`. |
| No se envía el Word por WhatsApp | Use **Enviar expediente Word** y elija WhatsApp en el menú; si el equipo no lo permite, el archivo se descarga y puede adjuntarse manualmente. |
| Cambié de celular | Los expedientes no se transfieren solos: antes de cambiar, comparta los Word y descargue el respaldo del mes. |

---
Basado en SHI-FOR-41 Rev. 03 · NOM-030-STPS-2009 · Guías IMSS ELSSA · Principios directivos OIT sobre vigilancia de la salud de los trabajadores.

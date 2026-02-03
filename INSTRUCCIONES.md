# 🚀 Instrucciones de Uso - App Transcripción FONATUR

## ⚠️ IMPORTANTE: Cómo Abrir la Aplicación

**NO** abras el archivo `index.html` directamente haciendo doble clic.

### Opción 1: Usar Live Server (Recomendado)

Si usas VS Code:

1. Instala la extensión "Live Server"
2. Clic derecho en `index.html` → "Open with Live Server"
3. Se abrirá en `http://127.0.0.1:5500/`

### Opción 2: Usar Python (Simple)

Abre una terminal en la carpeta `App_Alertas` y ejecuta:

```bash
# Python 3
python -m http.server 8000
```

Luego abre en tu navegador: `http://localhost:8000`

### Opción 3: Usar Node.js

Si tienes Node instalado:

```bash
npx serve
```

## 🔑 Configuración Inicial

1. **Obtén tu API Key de Gemini:**
   - Ve a https://aistudio.google.com/apikey
   - Inicia sesión con tu cuenta de Google
   - Crea una nueva API key (es GRATIS)
2. **Configura la API Key en la app:**
   - Haz clic en el ícono de llave (⚙️) en la esquina superior derecha
   - Pega tu API key
   - Clic en "Guardar"

## 📝 Uso

### Grabar Audio en Vivo

1. Haz clic en **"GRABAR"**
2. Permite el acceso al micrófono
3. Habla claramente
4. Haz clic en **"DETENER"**
5. Espera la transcripción

### Cargar Archivo de Audio

1. Haz clic en el ícono de **upload** (📤)
2. Selecciona un archivo MP3, WAV, WebM, etc.
3. Espera el procesamiento

**Formatos soportados:**

- MP3 ✅
- WAV ✅
- WebM ✅
- AAC ✅
- OGG ✅
- FLAC ✅

**Tamaño máximo:** ~20MB

## 🐛 Solución de Problemas

### "No hace nada al hacer clic"

- **Causa:** Abriste el archivo directamente con `file://`
- **Solución:** Usa un servidor HTTP local (ver arriba)

### "Error: Failed to fetch"

- **Causa:** No hay conexión a internet o la API key es inválida
- **Solución:** Verifica tu conexión y API key

### "Micrófono no permitido"

- **Causa:** No diste permiso al navegador
- **Solución:** Permite el acceso al micrófono en la configuración del navegador

### Error en consola: "CORS" o "importmap"

- **Causa:** Archivo abierto directamente sin servidor
- **Solución:** ¡Usa un servidor HTTP local!

## 💡 Consejos

- Para mejores resultados, habla claro y sin ruido de fondo
- Archivos más cortos (< 5 min) procesan más rápido
- Puedes configurar ejemplos de estilo en el ícono de libro (📖)
- El historial se guarda automáticamente en tu navegador

---

**¿Problemas?** Abre la consola del navegador (F12) y revisa los errores.

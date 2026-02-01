# Configuración de Notificaciones por Email - El Cónclave de San Martín

## Pasos para recibir emails cuando alguien complete el formulario

### 1. Configuración en Netlify (después de subir tu sitio)

Una vez que hayas subido tu sitio a Netlify, sigue estos pasos:

1. **Accede a tu panel de Netlify**
   - Ve a https://app.netlify.com
   - Selecciona tu sitio "El Cónclave de San Martín"

2. **Configura las notificaciones de formularios**
   - En el menú lateral, ve a: **Forms**
   - Verás el formulario "conclave-contact" después de que alguien lo envíe por primera vez
   - Haz clic en **Settings & notifications**
   - En la sección **Email notifications**, añade tu email

3. **Activa las notificaciones**
   - Marca la casilla "Email me when a new submission is received"
   - Guarda los cambios

### 2. Información que recibirás en cada email

Cada vez que alguien complete el formulario, recibirás un email con:

- **Nombre** del solicitante
- **Email profesional**
- **Empresa**
- **Teléfono**
- **Número de personas** (incluyendo si son más de 15)
- **Objetivos** que quieren conseguir
- **Servicios opcionales** seleccionados:
  - Transporte (si/no)
  - Restaurante (si/no)
  - Sala de reuniones (si/no)
- **Fecha preferida** para la experiencia

### 3. Actualiza tu email

En el archivo `netlify.toml`, cambia esta línea:
```
email = "tu-email@ejemplo.com"
```

Por tu email real, por ejemplo:
```
email = "info@elconclave.com"
```

### 4. Verificación Anti-Spam

El formulario incluye:
- **Honeypot** (trampa invisible para bots)
- **reCAPTCHA** de Google (opcional, ya configurado)

Esto te protege de spam automático.

### Notas importantes:

- La primera vez que alguien envíe el formulario, Netlify lo detectará automáticamente
- No necesitas configurar nada más en el código
- Los formularios de Netlify son gratuitos hasta 100 envíos al mes
- Si necesitas más, puedes actualizar tu plan de Netlify

¿Necesitas ayuda? Contacta con soporte de Netlify o conmigo.

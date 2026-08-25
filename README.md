# SinFiltro

Un muro donde cualquiera puede publicar de forma anónima un mensaje corto sobre cómo se siente, y leer los de los demás. Sin registro y sin cuentas.

**En vivo:** https://sinfiltro-a348f.web.app

## Tecnologías

- HTML5
- CSS3
- JavaScript
- Firebase Firestore
- Firebase Hosting

## Qué tiene de particular

- Los mensajes se insertan con `textContent`, nunca con `innerHTML`: es lo que impide que alguien publique código y lo ejecute en el navegador de los demás visitantes.
- **Reglas de seguridad de Firestore** que validan la forma de cada mensaje en el servidor, permiten sumar «me gusta» de uno en uno y prohíben editar o borrar publicaciones ajenas.
- Contador de personas conectadas con limpieza automática de sesiones caducadas.
- Política de privacidad que contempla el artículo 9 del RGPD, porque un mensaje sobre cómo te sientes puede contener datos de salud.

## Estructura

```
firebase.json     Configuración de Firebase Hosting y cabeceras de caché
.firebaserc       A qué proyecto de Firebase se despliega
public/           Todo lo que se publica
```

## Cómo desplegarlo

```bash
firebase deploy
```

---

Hecho por **Marcos Martínez** — desarrollador web en Valencia.

# Vinga Connect

Prototipo interactivo de una app para **Vinga Folkhögskola** (Frihamnen 15, Göteborg), desarrollado por **SJU Solutions**.
*En digital mötesplats för alla deltagare på Vinga – resan börjar här.*

Todo está en un único archivo, [`index.html`](index.html): HTML, CSS y JavaScript, sin dependencias ni fuentes externas. Así funciona incrustado en **Google Sites**.

## Qué incluye

| Pestaña | Contenido |
|---|---|
| **Puls** | Clase de hoy según el horario (aula, asignatura y botón al mapa), salidas de Västtrafik desde Frihamnen, aviso del día, eventos con "Jag kommer", votaciones del consejo de clase y de escuela, historias de Instagram y muro con palabras *lättläst* y traducción |
| **Studier** | Ruta de estudios real (SFI B → C → D → SAS Grund → Gymnasienivå), asistencia, puntos, *Dagens svenska* con voz, ranking de compañeros de idiomas y enlaces a Classroom, Drive, SchoolSoft, Exam.net y Deltagarsidor |
| **Chatt** | Fika-ruleta voluntaria, alumnos nuevos con botón de bienvenida, sugerencias Språkkompis, grupos y chats privados con solicitud previa, traducción por mensaje, frases rápidas en sueco, mensajes de voz, denunciar, bloquear y normas |
| **Guide** | Plano interactivo de la planta 3, aviso de ausencia (Sjukanmälan/VAB), "Bra att veta", contacto de la escuela y guía de Gotemburgo con los logos oficiales |
| **Profil** | Carné de estudiante con QR, "Sobre mí" (idiomas, intereses, privacidad), programa de padrinos, estudio de foto y avatar, e idiomas |

**Además:**
- **Ajustes:** notificaciones por tipo, tema, idioma, quién ve tu perfil, personas bloqueadas, descargar mis datos, política de privacidad, contacto y **borrar cuenta** (lo exigen App Store y Google Play).
- **Centro de notificaciones:** la campana con el contador de no leídos. Cada aviso lleva a su sitio, y hay avisos tipo push cuando llega un mensaje.
- **Bienvenida de primera vez:** 4 pasos para elegir idioma, presentar la app, indicar tus idiomas y dar permiso para las notificaciones.
- **Modo oscuro:** automático según el teléfono, o claro u oscuro a mano.
- **8 idiomas:** svenska, español, English, العربية, فارسی, Türkçe, українська y русский. Árabe y persa se muestran de derecha a izquierda.
- Se adapta al móvil (pantalla completa) y al escritorio (marco de teléfono).

## Probar en local

```bash
python -m http.server 8000
```

Abre `http://localhost:8000`. Para probarlo en el móvil, conéctalo a la misma red wifi y abre `http://<IP-del-ordenador>:8000`.

## Usar en Google Sites

Ve a **Insertar → Insertar → Código insertado** y pega todo el contenido de `index.html`. Si quieres ver el marco de teléfono, usa una altura de unos 860 px.

## Importante

- **Es un prototipo.** Los horarios, las aulas, los mensajes, las personas, los eventos y las votaciones son **datos de demostración ficticios**. No se envía ni se guarda nada en ningún servidor; solo el idioma elegido se recuerda en el navegador.
- Los datos de la escuela (programas, horarios de SFI, fechas del curso, contacto y enlaces) salen de [vingafolkhogskola.se](https://vingafolkhogskola.se/) y se leyeron en noviembre de 2026.
- Los logos de Google Classroom, Google Drive, Västtrafik, 1177, CSN, Arbetsförmedlingen y Skatteverket pertenecen a sus respectivos titulares. Solo se usan para enlazar a sus servicios.
- La versión real necesitaría la aprobación de la escuela, cuentas de Google Workspace, conexión con SchoolSoft, moderación del chat y protección de datos (RGPD).

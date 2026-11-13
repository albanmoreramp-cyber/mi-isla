# mi-isla

**Una isla dinámica para Windows**, inspirada en la Dynamic Island del iPhone, que vive en la parte de arriba de la pantalla y te muestra de un vistazo la música, el volumen, tu agenda, el correo y los avisos de Claude.

![Vista general de mi-isla](docs/portada.png)

> ADVERTENCIA: **Programa gratuito para uso personal.** No es de código abierto: aquí se publica la aplicación lista para usar y su documentación, no el código fuente.

---

## ¿Qué es?

mi-isla es una pequeña barra flotante, siempre encima del resto de ventanas, pegada al borde superior. **Plegada** ocupa muy poco y te enseña solo lo justo; cuando **pasas el ratón por encima** se despliega y se convierte en un panel con pestañas. Está pensada para tenerla ahí todo el día sin molestar.

## Funciones

### Con la isla plegada
- **Reloj**, con la información que elijas a los lados (batería, CPU, RAM, Wi-Fi, Bluetooth o la fecha).
- **Música en directo**: carátula del disco y **letra sincronizada** que avanza línea a línea con la canción. Las barritas y la luz de la barra toman el color de la carátula.
- **Barra de volumen** cuando lo subes o lo bajas.
- **Avisos de la app de Claude** y de los archivos que llegan desde el móvil.
- Se puede **esconder** en una línea fina, y **desaparece sola** cuando ves un vídeo o juegas a pantalla completa.

### Con la isla desplegada (pasa el ratón por encima)
- **Inicio** — un reloj grande personalizable (tipografía, grosor y color, o el color del disco que suena) y tres tarjetas con la música, Claude y tu día.
- **Música** — carátula a lo grande, letra, barra de progreso para saltar a cualquier punto, controles y volumen.
- **Agenda** — tu Google Calendar: vista de día con línea de tiempo, vista de mes y un botón para crear eventos.
- **Correo** — tu Gmail: cuántos correos sin leer tienes y los últimos (remitente y asunto).
- **Claude** — los últimos avisos de la app de escritorio de Claude.
- **Bandeja** — guarda archivos arrastrándolos a la isla y **pásalos al móvil** con un código QR.

En la cabecera tienes también **Wi-Fi y Bluetooth** (encenderlos, ver redes y conectarte) y un menú con el volumen, personalización, ajustes y salir.

![La pestaña de Música con la carátula y la letra](docs/musica.png)

## Cómo funciona

- Está hecha con **Electron** (es decir, es una app de escritorio hecha con tecnología web).
- La **música** la lee de los controles multimedia del propio Windows, así que funciona con Spotify, los navegadores y casi cualquier reproductor. La **letra** se busca en LRCLIB (lrclib.net), un servicio gratuito; si no la encuentra ahí, muestra el título y el artista. Si Windows no da la carátula, la busca en el catálogo público de iTunes.
- La **agenda y el correo** se conectan a tu cuenta de Google con tu permiso. Solo puede ver y crear eventos y leer el remitente y el asunto de los correos, **nunca su contenido**.
- Los **avisos de Claude** se leen de las notificaciones que la app de Claude envía a Windows.
- El **paso al móvil** abre una conexión temporal en tu red Wi-Fi (con una dirección secreta dentro del QR) que se cierra sola al cabo de una hora.

![Inicio y Ajustes](docs/inicio.png)

## Instalación

1. Ve a la sección Releases (en la pestaña superior del repositorio) y descarga `mi-isla.exe`.
2. Haz **doble clic**. No hay que instalar nada: es un programa portátil.
3. La primera vez tarda unos segundos en aparecer arriba. Vive en el icono junto al reloj de Windows.

### Aviso de seguridad al abrirlo

Como la aplicación **no está firmada con un certificado de pago**, la primera vez Windows puede mostrar la pantalla azul **"Windows protegió su PC"**. Es lo normal en cualquier programa casero y no significa que tenga nada malo.

Para abrirla: pulsa **"Más información"** y luego **"Ejecutar de todas formas"**.

## Requisitos

- Windows 10 u 11 (64 bits).

## Atajos

- **Ctrl + Alt + I** — mostrar u ocultar la isla.
- **Esc** — plegarla.

## Privacidad

Todo ocurre en tu propio ordenador. Tus ajustes y la sesión de Google se guardan **cifrados con tu usuario de Windows** en una carpeta tuya (`.mi-isla`). Nada se envía a ningún servidor del autor.

## Licencia

Software propietario. Todos los derechos reservados. Consulta el archivo LICENSE. El código fuente no se publica y el programa se distribuye con el código **ofuscado**.

## Créditos

Creado por **Albán Morera** · alban@gmail.com

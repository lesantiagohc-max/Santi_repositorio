# **Proyecto de Santiago Herrera Conde**

Bienvenido  😁

Soy **Santiago Herrera Conde**, estudiante de la Ingenieria en Mecatronica en la **IBERO Puebla**, actualmente curso 1.er semestre.
---
<img>scr="https://github.com/lesantiagohc-max/Santi_repositorio/blob/main/docs/recursos/imgs/imagen%20pagina%20meca.jpg"
---

**Un poco de mi:**

Me considero alguien creativo y siempre dispuesto a enfretar nuevos retos.

Entre mis gustos se encuentran los deportes como el futbol, el hockey sobre pasto y el boxeo, tambien me gustan mucho los videojuegos especializados en shooters u juegos de simulacion, a su vez tengo una gran pasion por la cocina, estas actividades no solo las disfruto, sino que tambien me ayudan a crecer como persona dia tras dia.

Considero que uno de mis mayores logros ha sido pertenecer al seleccionado estatal del equipo de hockey de Tlaxcala, al igual que haber participado en distintos torneos estatales y nacionales de futbol.

---
Contacto: 201239@iberopuebla.mx
---

<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Reloj Digital Moderno 12h — Ciudad de México</title>
<style>

  .reloj {
    background: rgba(0,0,0,0.4); /* fondo semi-transparente */
    backdrop-filter: blur(10px);
    padding: 40px 60px;
    border-radius: 20px;
    text-align: center;
    box-shadow: 0 8px 25px rgba(0,0,0,0.6);
    color: #fff;
    min-width: 280px;
  }

  .hora {
    font-size: 60px;
    font-weight: 700;
    letter-spacing: 2px;
    margin-bottom: 15px;
  }

  .fecha {
    font-size: 18px;
    color: #cfd8dc;
    text-transform: capitalize;
  }

  @media(max-width: 400px){
    .reloj {
      padding: 30px 40px;
    }
    .hora { font-size: 45px; }
    .fecha { font-size: 16px; }
  }
</style>
</head>
<body>

<div class="reloj">
  <div id="hora" class="hora">--:--:-- --</div>
  <div id="fecha" class="fecha">Cargando fecha...</div>
</div>

<script>
const TIMEZONE = 'America/Mexico_City';

function actualizarReloj() {
  const ahora = new Date();

  // Hora en formato 12h con AM/PM
  const horaStr = new Intl.DateTimeFormat('es-MX', {
    timeZone: TIMEZONE,
    hour: '2-digit',
    minute: '2-digit',
    second: '2-digit',
    hour12: true
  }).format(ahora);

  // Fecha completa en español
  const fechaStr = new Intl.DateTimeFormat('es-MX', {
    timeZone: TIMEZONE,
    weekday: 'long',
    day: 'numeric',
    month: 'long',
    year: 'numeric'
  }).format(ahora);

  document.getElementById('hora').textContent = horaStr;
  document.getElementById('fecha').textContent = fechaStr;
}

// Ejecutar al cargar y actualizar cada segundo
actualizarReloj();
setInterval(actualizarReloj, 1000);
</script>

</body>
</html>
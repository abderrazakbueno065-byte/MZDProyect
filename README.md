<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>MZD Dental - Prótesis Dentales</title>

<!-- Font Awesome para iconos -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

<style>
*{
  margin:0;
  padding:0;
  box-sizing:border-box;
  font-family:Arial, Helvetica, sans-serif;
  scroll-behavior:smooth;
}

/* BODY */
body{
  background:#f5fbff;
}

/* NAVBAR */
header{
  position:fixed;
  top:0;
  width:100%;
  display:flex;
  justify-content:space-between;
  align-items:center;
  padding:20px 60px;
  background:white;
  box-shadow:0 2px 10px rgba(0,0,0,0.1);
  z-index:10;
}

.logo{
  font-size:28px;
  font-weight:bold;
  color:#0077b6;
}

.btnCita{
  background:#0077b6;
  color:white;
  border:none;
  padding:12px 22px;
  border-radius:25px;
  cursor:pointer;
  font-size:15px;
}

.btnCita:hover{
  background:#005f8f;
}

/* HERO */
.hero{
  height:100vh;
  display:flex;
  align-items:center;
  justify-content:center;
  text-align:center;
  background-image: url("protesis-dentales.jpg");
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  position:relative;
}

.hero::before{
  content:"";
  position:absolute;
  top:0;
  left:0;
  width:100%;
  height:100%;
  background:rgba(0,0,0,0.4);
}

.hero div{
  position:relative;
  color:white;
  text-shadow: 2px 2px 6px rgba(0,0,0,0.6);
}

.hero h1{
  font-size:50px;
}

.hero p{
  margin-top:15px;
  font-size:18px;
}

.hero .btnCitaHero{
  margin-top:20px;
  padding:15px 30px;
  font-size:18px;
  border-radius:30px;
  background:#00b4d8;
  border:none;
  cursor:pointer;
  transition:0.3s;
}

.hero .btnCitaHero:hover{
  background:#0096c7;
}

/* SECCIONES */
section{
  padding:100px 60px;
}

section:nth-of-type(even){
  background:#f0f8ff;
}

.titulo{
  text-align:center;
  margin-bottom:50px;
  font-size:40px;
  color:#023e8a;
}

/* SOBRE NOSOTROS */
.sobre{
  max-width:900px;
  margin:auto;
  text-align:center;
  font-size:18px;
  color:#444;
}

/* SERVICIOS */
.serviciosGrid{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
  gap:30px;
}

.servicio{
  background:white;
  padding:30px;
  border-radius:15px;
  box-shadow:0 10px 20px rgba(0,0,0,0.08);
  text-align:center;
}

.servicio i{
  margin-bottom:10px;
}

.servicio h3{
  color:#0077b6;
  margin-bottom:10px;
}

/* FORMULARIO */
.formContainer{
  display:flex;
  justify-content:center;
}

form{
  background:white;
  padding:40px;
  border-radius:15px;
  width:350px;
  box-shadow:0 10px 25px rgba(0,0,0,0.1);
}

form input{
  width:100%;
  padding:10px;
  margin-bottom:15px;
  border-radius:8px;
  border:1px solid #ccc;
}

form button{
  width:100%;
  padding:12px;
  background:#0077b6;
  color:white;
  border:none;
  border-radius:10px;
  cursor:pointer;
  font-size:16px;
}

/* FOOTER */
footer{
  background:#023e8a;
  color:white;
  text-align:center;
  padding:30px;
  margin-top:40px;
}

footer .redes a{
  color:white;
  margin:0 10px;
  font-size:20px;
  transition:0.3s;
}

footer .redes a:hover{
  color:#00b4d8;
}

/* RESPONSIVE */
@media(max-width:768px){
  header{
    padding:20px;
    flex-direction:column;
  }
  .hero h1{
    font-size:36px;
  }
  .hero p{
    font-size:16px;
  }
  form{
    width:90%;
  }
  section{
    padding:60px 20px;
  }
}

</style>
</head>
<body>

<!-- NAVBAR -->
<header>
  <div class="logo">MZD Dental</div>
  <button class="btnCita" onclick="irFormulario()">Pedir Cita Ahora</button>
</header>

<!-- HERO -->
<section class="hero">
  <div>
    <h1>MZD Dental</h1>
    <p>Laboratorio de Prótesis Dentales<br>Mohamed Zaidi Dfouf</p>
    <button class="btnCitaHero" onclick="irFormulario()">Reservar Cita</button>
  </div>
</section>

<!-- SOBRE NOSOTROS -->
<section>
  <h2 class="titulo">Sobre Nosotros</h2>
  <p class="sobre">
    En MZD Dental nos especializamos en la fabricación de prótesis dentales
    de alta calidad diseñadas para restaurar la función y la estética de la sonrisa.
    Trabajamos con tecnología moderna para ofrecer soluciones personalizadas
    a cada paciente.
  </p>
</section>

<!-- TIPOS DE PROTESIS -->
<section>
  <h2 class="titulo">Tipos de Prótesis Dentales</h2>
  <div class="serviciosGrid">
    <div class="servicio">
      <i class="fa-solid fa-tooth fa-2x" style="color:#0077b6;"></i>
      <h3>Prótesis Removibles</h3>
      <p>Prótesis que el paciente puede retirar fácilmente para su limpieza. Incluyen prótesis acrílicas, esqueléticas y flexibles.</p>
    </div>
    <div class="servicio">
      <i class="fa-solid fa-tooth fa-2x" style="color:#0077b6;"></i>
      <h3>Prótesis Fijas</h3>
      <p>Se colocan permanentemente sobre dientes naturales o implantes, ofreciendo mayor estabilidad y comodidad.</p>
    </div>
    <div class="servicio">
      <i class="fa-solid fa-tooth fa-2x" style="color:#0077b6;"></i>
      <h3>Prótesis Completas</h3>
      <p>Sustituyen todos los dientes de la arcada dental cuando el paciente ha perdido la dentadura completa.</p>
    </div>
    <div class="servicio">
      <i class="fa-solid fa-tooth fa-2x" style="color:#0077b6;"></i>
      <h3>Prótesis Parciales</h3>
      <p>Sustituyen uno o varios dientes mientras se conservan los dientes naturales restantes.</p>
    </div>
  </div>
</section>

<!-- FORMULARIO -->
<section id="formulario">
  <h2 class="titulo">Reservar Cita</h2>
  <div class="formContainer">
    <form>
      <input type="text" placeholder="Nombre" required>
      <input type="text" placeholder="Apellidos" required>
      <input type="email" placeholder="Correo electrónico" required>
      <input type="date" required>
      <input type="time" required>
      <button>Reservar Cita</button>
    </form>
  </div>
</section>

<!-- FOOTER -->
<footer>
  <div>
    <p>MZD Dental © 2026</p>
    <p>Mohamed Zaidi Dfouf</p>
    <div class="redes">
      <a href="#"><i class="fa-brands fa-facebook-f"></i></a>
      <a href="#"><i class="fa-brands fa-instagram"></i></a>
      <a href="#"><i class="fa-brands fa-whatsapp"></i></a>
    </div>
  </div>
</footer>

<!-- SCRIPT -->
<script>
function irFormulario(){
  document.getElementById("formulario").scrollIntoView({
    behavior:"smooth"
  });
}
</script>

</body>
</html>

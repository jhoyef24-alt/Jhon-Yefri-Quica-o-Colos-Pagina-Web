<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Portafolio - Jhon Yefri</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
<style>
    * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Poppins', sans-serif; }
    body {
        background: #0f0f0f;
        color: #e8e8e8;
    }

    /* NAVBAR MODERNA */
    .navbar {
        width: 100%;
        padding: 15px 0;
        background: rgba(0,0,0,0.7);
        backdrop-filter: blur(10px);
        position: sticky;
        top: 0; z-index: 1000;
        display: flex; justify-content: center; gap: 30px;
    }
    .navbar button {
        background: none;
        border: none;
        color: #00ff9d;
        font-size: 18px;
        cursor: pointer;
        font-weight: 600;
        transition: 0.3s;
    }
    .navbar button:hover, .navbar .active-tab {
        color: white;
        text-shadow: 0 0 8px #00ff9d;
    }

    /* HERO SECTION */
    header {
        text-align: center;
        padding: 80px 20px;
        background: radial-gradient(circle at top, #00ff9d20, #000000 70%);
    }
    header img {
        width: 160px; height: 160px;
        border-radius: 50%; border: 4px solid #00ff9d;
        box-shadow: 0 0 20px #00ff9d60;
    }
    header h1 { margin-top: 20px; font-size: 38px; font-weight: 600; }
    header p { font-size: 18px; opacity: 0.8; }

    /* CONTENIDO */
    .tab-content {
        display: none;
        width: 90%; max-width: 900px;
        margin: 40px auto;
        background: #1a1a1a;
        padding: 30px;
        border-radius: 16px;
        box-shadow: 0 0 20px rgba(33, 184, 121, 0.08);
        animation: fade 0.5s ease;
    }
    @keyframes fade { from {opacity:0; transform: translateY(10px);} to {opacity:1; transform: translateY(0);} }

    h2 { font-size: 26px; margin-bottom: 15px; color: #00ff9d; }

    ul li { margin: 10px 0; }

    footer {
        text-align: center;
        padding: 20px;
        margin-top: 60px;
        background: #000;
        color: #888;
        .icon-btn {
    width: 55px;
    height: 55px;
    background: #ffffff;
    border-radius: 10px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    cursor: pointer;
    transition: 0.3s;
    border: none;
    box-shadow: 0 0 10px #00ff9d40;
    font-size: 13px;
    color: #000;
    text-decoration: none;
}

.icon-btn:hover {
    transform: scale(1.05);
    box-shadow: 0 0 15px #00ff9d90;
}

.icon-symbol {
    font-size: 22px;
    margin-bottom: 4px;
}

    }
</style>
</head>
<body>

<!-- NAVBAR -->
<div class="navbar">
    <button onclick="openTab('sobre-mi')" id="btn-sobre">Sobre mí</button>
    <button onclick="openTab('educacion')" id="btn-educacion">Educación</button>
    <button onclick="openTab('experiencia')" id="btn-experiencia">Experiencia</button>
    <button onclick="openTab('actividades')" id="btn-actividades">Actividades</button>
    <button onclick="openTab('habilidades')" id="btn-habilidades">Habilidades</button>
    <button onclick="openTab('contacto')" id="btn-contacto">Contacto</button>
</div>

<!-- HERO -->
<header>
    <img src="foto-perfil.jpg" alt="foto-perfil" />
    <h1>Jhon Yefri Quicaño Colos</h1>
    <p>Estudiante de Derecho – IX Ciclo</p>
<div style="display:flex; gap:15px; justify-content:center; margin-top:20px;">
    
    <!-- BOTÓN MODO -->
    <button class="icon-btn" onclick="toggleTheme()">
        <span class="icon-symbol">◐</span>
        Modo
    </button>

    <!-- BOTÓN DESCARGAR CV -->
    <a href="CV-JhonYefri.pdf" download style="display:flex; align-items:center; text-decoration:none; color:white;">
    <div class="cv-icon-box">📄</div>
    <span>CV</span>
</div>

</header>

<!-- TAB SECTIONS -->
<section id="sobre-mi" class="tab-content">
    <h2>Sobre mí</h2>
    <p>Soy estudiante del IX ciclo de Derecho con interés en las áreas del derecho Administrativo, Ambiental y Penal. Me caracterizo por mi liderazgo, proactividad y compromiso con el aprendizaje continuo.</p>
</section>

<section id="educacion" class="tab-content">
    <h2>Educación</h2>
    <ul>
        <li><strong>Universidad Científica del Sur</strong> – IX ciclo</li>
        <li><strong>Centro de Idiomas – Científica del Sur</strong> – Inglés básico</li>
        <li><strong>CENAN Perú</strong> – Gerencia Pública</li>
        <li><strong>Curso de Excel Avanzado</strong></li>
    </ul>
</section>

<section id="experiencia" class="tab-content">
    <h2>Experiencia Profesional</h2>
    <ul>
        <li>Asistente Administrativo – Hinostroza & Asociados (2024)</li>
        <li>Asistente Legal – Hinostroza & Asociados (2025)</li>
        <li>Voluntariado – Ministerio Público</li>
        <li>Mentor Beca 18 – Pronabec (2024 – 2025)</li>
    </ul>
</section>

<section id="actividades" class="tab-content">
    <h2>Actividades Extracurriculares</h2>
    <ul>
        <li>Exmiembro de Lex Sphere – Área audiovisual</li>
        <li>Congreso de Derecho Ambiental (2024)</li>
        <li>Desafío Arbitral – UCSB</li>
        <li>Taller de Habilidades Blandas – Pronabec</li>
    </ul>
</section>

<section id="habilidades" class="tab-content">
    <h2>Habilidades</h2>
    <p>Liderazgo • Comunicación asertiva • Resolución de problemas • Proactividad • Adaptabilidad • Trabajo en equipo</p>
</section>

<section id="contacto" class="tab-content">
    <h2>Contacto</h2>
    <p>📞 929118941</p>
    <p>📧 jhonyefriq@gmail.com</p>
    <p>📍 San Juan de Miraflores, Lima – Perú</p>
</section>

<!-- SCRIPT DE TABS -->
<script>
function openTab(id){
    document.querySelectorAll('.tab-content').forEach(t => t.style.display = 'none');
    document.getElementById(id).style.display = 'block';

    document.querySelectorAll('.navbar button').forEach(b => b.classList.remove('active-tab'));
    document.getElementById('btn-' + id).classList.add('active-tab');
}

// Tab inicial
openTab('sobre-mi');
</script>

<script>
const toggle=document.getElementById('themeToggle');
toggle.onclick=()=>{
 document.body.classList.toggle('light');
};
</script>
<footer class="footer-redes">
    <a href="https://www.facebook.com/jhonyefri.quicanocolos/" target="_blank" class="icono-red">
        <svg xmlns="https://www.facebook.com/" width="22" height="22" fill="currentColor" viewBox="0 0 24 24">
            <path d="M22.675 0h-21.35C.597 0 0 .597 0 1.326v21.348C0 23.403.597 24 1.325 
                     24h11.495v-9.294H9.691v-3.622h3.129V8.413c0-3.1 1.893-4.788 
                     4.659-4.788 1.325 0 2.464.099 2.795.143v3.24l-1.918.001c-1.504 
                     0-1.795.715-1.795 1.764v2.313h3.587l-.467 3.622h-3.12V24h6.116C23.403 
                     24 24 23.403 24 22.674V1.326C24 .597 23.403 0 22.675 0z"/>
        </svg>
    </a>

    <a href="https://www.instagram.com/jhonyefriqc/" target="_blank" class="icono-red">
        <svg xmlns="http://www.w3.org/2000/svg" width="22" height="22" fill="currentColor" viewBox="0 0 24 24">
            <path d="M12 2.163c3.204 0 3.584.012 4.85.07 1.17.056 1.97.24 2.427.403a4.92 
                     4.92 0 0 1 1.75 1.145 4.92 4.92 0 0 1 1.145 1.75c.163.457.347 
                     1.257.403 2.427.058 1.266.07 1.646.07 4.85s-.012 3.584-.07 
                     4.85c-.056 1.17-.24 1.97-.403 2.427a4.92 4.92 0 0 1-1.145 
                     1.75 4.92 4.92 0 0 1-1.75 1.145c-.457.163-1.257.347-2.427.403-1.266.058-1.646.07-4.85.07s-3.584-.012-4.85-.07c-1.17-.056-1.97-.24-2.427-.403a4.92 
                     4.92 0 0 1-1.75-1.145 4.92 4.92 0 0 1-1.145-1.75c-.163-.457-.347-1.257-.403-2.427C2.175 
                     15.584 2.163 15.204 2.163 12s.012-3.584.07-4.85c.056-1.17.24-1.97.403-2.427A4.92 
                     4.92 0 0 1 3.781 2.973a4.92 4.92 0 0 1 1.75-1.145c.457-.163 1.257-.347 
                     2.427-.403C8.416 2.175 8.796 2.163 12 2.163zm0 3.675a6.162 
                     6.162 0 1 0 0 12.324 6.162 6.162 0 0 0 0-12.324zm7.2-1.35a1.44 
                     1.44 0 1 0 0 2.88 1.44 1.44 0 0 0 0-2.88z"/>
        </svg>
    </a>

    <a href="https://wa.me/51TU_929118941" target="_blank" class="icono-red">
        <svg xmlns="http://www.w3.org/2000/svg" width="22" height="22" fill="currentColor" viewBox="0 0 24 24">
            <path d="M20.52 3.48A11.87 11.87 0 0 0 12.04 0C5.46 0 .28 5.17.28 11.74c0 
                     2.07.54 4.09 1.57 5.88L0 24l6.53-1.71a11.7 11.7 0 0 0 5.51 
                     1.4h.01c6.58 0 11.75-5.17 11.75-11.74 0-3.13-1.22-6.07-3.28-8.21zM12.05 
                     21.3h-.01a9.6 9.6 0 0 1-4.9-1.34l-.35-.21-3.87 1.02 1.04-3.77-.23-.39a9.54 
                     9.54 0 0 1-1.46-5.1c0-5.28 4.3-9.57 9.6-9.57 2.56 0 4.97 1 6.78 
                     2.82a9.48 9.48 0 0 1 2.81 6.75c0 5.28-4.3 9.58-9.6 9.58zm5.44-7.23c-.3-.15-1.77-.87-2.04-.97-.27-.1-.47-.15-.67.15-.2.3-.77.97-.94 
                     1.17-.17.2-.35.22-.65.07-.3-.15-1.26-.46-2.4-1.47-.89-.79-1.49-1.77-1.66-2.07-.17-.3-.02-.46.13-.61.14-.14.3-.35.44-.52.15-.17.2-.3.3-.5.1-.2.05-.37-.02-.52-.07-.15-.67-1.61-.92-2.2-.24-.58-.49-.5-.67-.51-.17-.01-.37-.01-.57-.01-.2 
                     0-.52.07-.8.37-.27.3-1.05 1.03-1.05 2.5s1.08 2.9 1.23 3.11c.15.2 2.13 3.25 5.16 
                     4.56.72.31 1.28.5 1.72.64.72.23 1.38.2 1.9.12.58-.09 1.77-.72 
                     2.02-1.41.25-.69.25-1.28.17-1.41-.07-.13-.27-.2-.57-.35z"/>
        </svg>
    </a>

    <a href="https://www.linkedin.com/in/jhon-yefri-quica%C3%B1o-colos-200871224/" target="_blank" class="icono-red">
        <svg xmlns="http://www.w3.org/2000/svg" width="22" height="22" fill="currentColor" viewBox="0 0 24 24">
            <path d="M4.98 3.5a2.5 2.5 0 1 1-.01 5.01 2.5 2.5 0 0 1 
                     .01-5.01zM.5 8.98h8.91v14.52H.5V8.98zm9.99 
                     0h8.54v2.07h.12c1.19-2.25 4.1-2.31 5.33-.44 1.22 1.86.98 5.22.98 
                     7.9v8.99h-8.9v-7.97c0-1.9-.03-4.34-2.64-4.34-2.64 0-3.04 
                     2.06-3.04 4.2v8.11H10.5V8.98z"/>
        </svg>
    </a>
</footer>

</body>
</html>

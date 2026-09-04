<script setup lang="ts">
// Rigel S.A. - Portafolio Comercial y Verificación
</script>

<template>
  <div class="smooth-scroll-wrapper">
    <!-- HERO SECTION -->
    <section class="hero">
      <div class="hero-bg" style="background-image: url('/images/hero-rigel.jpg');"></div>
      <div class="hero-overlay"></div>

      <nav class="nav">
        <div class="logo">RIGEL.</div>
        <a href="#contacto" class="btn-contact">Hablemos</a>
      </nav>

      <div class="hero-content">
        <div class="reveal-text">
          <h1 class="display-title">SOLUCIONES <br/> INDUSTRIALES & TI</h1>
        </div>
        <p class="hero-subtitle">Maquinaria, tecnología y consultoría especializada <br/> para impulsar tu negocio.</p>
      </div>

      <div class="scroll-indicator">
        <div class="mouse"></div>
        <span>Descubre</span>
      </div>
    </section>

    <!-- MARQUEE -->
    <div class="marquee-container">
      <div class="marquee">
        <span>MAQUINARIA INDUSTRIAL &mdash; EQUIPO INFORMÁTICO &mdash; CONSULTORÍA TI &mdash; GESTIÓN DE SISTEMAS &mdash; </span>
        <span>MAQUINARIA INDUSTRIAL &mdash; EQUIPO INFORMÁTICO &mdash; CONSULTORÍA TI &mdash; GESTIÓN DE SISTEMAS &mdash; </span>
      </div>
    </div>

    <!-- PORTFOLIO / GALLERY -->
    <section class="gallery">
      <div class="gallery-header">
        <h2 class="section-title">NUESTRA <br/> ESPECIALIDAD</h2>
        <p class="section-desc">Desde intermediación de maquinaria industrial hasta consultoría en sistemas informáticos. En RIGEL conectamos tecnología con resultados.</p>
      </div>

      <div class="gallery-grid">
        <div class="gallery-item large">
          <div class="image-wrapper">
            <img src="/images/maquinaria.jpg" alt="Maquinaria Industrial" />
            <div class="item-overlay">
              <h3>Intermediación</h3>
              <p>Maquinaria y Equipo Industrial</p>
            </div>
          </div>
        </div>
        <div class="gallery-item">
          <div class="image-wrapper">
            <img src="/images/tecnologia.jpg" alt="Consultoría TI" />
            <div class="item-overlay">
              <h3>Consultoría</h3>
              <p>Computadoras y Sistemas TI</p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- FOOTER / LEGAL INFO -->
    <footer id="contacto" class="legal-footer">
      <div class="footer-grid">
        <!-- Branding / Contact -->
        <div class="footer-col brand-col">
          <h2 class="footer-logo">RIGEL.</h2>
          <p class="contact-email"><a href="mailto:rigelecuadorsa@gmail.com">rigelecuadorsa@gmail.com</a></p>
          <div class="phones">
            <a href="tel:0995954964">0995954964</a>
          </div>
          <p class="copyright">&copy; {{ new Date().getFullYear() }} RIGEL S.A. All rights reserved.</p>
        </div>

        <!-- SRI Legal Data -->
        <div class="footer-col legal-data">
          <h4>Información Comercial y Tributaria</h4>
          <div class="data-grid">
            <div class="data-item">
              <span class="label">Razón Social</span>
              <span class="value">RIGEL S.A.</span>
            </div>
            <div class="data-item">
              <span class="label">RUC</span>
              <span class="value">0993385173001</span>
            </div>
            <div class="data-item">
              <span class="label">Representante</span>
              <span class="value">Hurtado Alvarez Juan Gabriel</span>
            </div>
            <div class="data-item">
              <span class="label">Estado / Régimen</span>
              <span class="value">Activo / General</span>
            </div>
            <div class="data-item">
              <span class="label">Actividades</span>
              <span class="value">Intermediación de maquinaria industrial, venta de computadoras y consultoría en sistemas informáticos.</span>
            </div>
            <div class="data-item">
              <span class="label">Fechas SRI</span>
              <span class="value">Constitución: 04/09/2023 | Inicio: 12/09/2023</span>
            </div>
            <div class="data-item">
              <span class="label">Verificación SRI</span>
              <span class="value">RCR1787064540973837</span>
            </div>
          </div>
        </div>

        <!-- Address -->
        <div class="footer-col address-col">
          <h4>Ubicación</h4>
          <p>
            Calle Elizalde 0119 y Malecón,<br>
            Edificio Luz María, Oficina B<br>
            (Diagonal al Banco Internacional)<br>
            Guayaquil, Guayas, Zona 8<br>
            Ecuador
          </p>

          <div class="tax-tags">
            <span class="tax-tag">IVA</span>
            <span class="tax-tag">Renta Sociedades</span>
            <span class="tax-tag">ATS</span>
            <span class="tax-tag">ADI</span>
            <span class="tax-tag">REBEFICS</span>
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Syne:wght@400;700;800&family=Inter:wght@300;400;500&display=swap');

$font-display: 'Syne', sans-serif;
$font-body: 'Inter', sans-serif;
$color-bg: #0a0a0a;
$color-text: #ffffff;
$color-accent: #f2295b;
$color-muted: #888888;

.smooth-scroll-wrapper {
  background-color: $color-bg;
  color: $color-text;
  font-family: $font-body;
  overflow-x: hidden;
  -webkit-font-smoothing: antialiased;
}

/* HERO SECTION */
.hero {
  position: relative;
  height: 100vh;
  width: 100vw;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  padding: 2rem 4rem;
  box-sizing: border-box;
  overflow: hidden;

  .hero-bg {
    position: absolute;
    top: 0; left: 0; right: 0; bottom: 0;
    background-size: cover;
    background-position: center;
    transform: scale(1.05);
    animation: slowZoom 20s infinite alternate linear;
    z-index: 1;
  }

  .hero-overlay {
    position: absolute;
    top: 0; left: 0; right: 0; bottom: 0;
    background: linear-gradient(180deg, rgba(0,0,0,0.3) 0%, rgba(0,0,0,0.8) 100%);
    z-index: 2;
  }

  .nav {
    position: relative;
    z-index: 10;
    display: flex;
    justify-content: space-between;
    align-items: center;

    .logo {
      font-family: $font-display;
      font-weight: 800;
      font-size: 1.5rem;
      letter-spacing: -0.02em;
    }

    .btn-contact {
      border: 1px solid rgba(255,255,255,0.3);
      padding: 0.75rem 1.5rem;
      border-radius: 50px;
      color: $color-text;
      text-decoration: none;
      font-size: 0.9rem;
      transition: all 0.3s ease;
      backdrop-filter: blur(5px);

      &:hover {
        background: $color-text;
        color: $color-bg;
      }
    }
  }

  .hero-content {
    position: relative;
    z-index: 10;
    margin-bottom: 10vh;

    .reveal-text {
      overflow: hidden;
      .display-title {
        font-family: $font-display;
        font-size: clamp(4rem, 12vw, 10rem);
        font-weight: 800;
        line-height: 0.9;
        margin: 0;
        text-transform: uppercase;
        letter-spacing: -0.04em;
        animation: revealUp 1s cubic-bezier(0.77, 0, 0.175, 1) forwards;
      }
    }

    .hero-subtitle {
      margin-top: 2rem;
      font-size: clamp(1rem, 2vw, 1.5rem);
      font-weight: 300;
      opacity: 0;
      animation: fadeIn 1s ease 1s forwards;
    }
  }

  .scroll-indicator {
    position: absolute;
    bottom: 2rem;
    left: 50%;
    transform: translateX(-50%);
    z-index: 10;
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 0.5rem;
    font-size: 0.8rem;
    text-transform: uppercase;
    letter-spacing: 0.1em;
    opacity: 0.7;

    .mouse {
      width: 20px;
      height: 30px;
      border: 1px solid white;
      border-radius: 10px;
      position: relative;

      &::after {
        content: '';
        position: absolute;
        top: 5px;
        left: 50%;
        transform: translateX(-50%);
        width: 2px;
        height: 5px;
        background: white;
        border-radius: 2px;
        animation: scrollWheel 2s infinite ease-in-out;
      }
    }
  }
}

/* MARQUEE */
.marquee-container {
  padding: 4rem 0;
  background: $color-accent;
  color: $color-bg;
  overflow: hidden;
  white-space: nowrap;

  .marquee {
    display: inline-block;
    animation: marqueeMove 20s linear infinite;
    
    span {
      font-family: $font-display;
      font-weight: 800;
      font-size: 3rem;
      padding-right: 1rem;
    }
  }
}

/* GALLERY */
.gallery {
  padding: 10vw 4rem;

  .gallery-header {
    margin-bottom: 5rem;
    display: flex;
    justify-content: space-between;
    align-items: flex-end;
    gap: 2rem;
    flex-wrap: wrap;

    .section-title {
      font-family: $font-display;
      font-size: clamp(3rem, 8vw, 6rem);
      line-height: 0.9;
      margin: 0;
    }

    .section-desc {
      max-width: 400px;
      font-size: 1.1rem;
      color: $color-muted;
      line-height: 1.6;
    }
  }

  .gallery-grid {
    display: grid;
    grid-template-columns: repeat(12, 1fr);
    gap: 2rem;

    .gallery-item {
      position: relative;
      overflow: hidden;
      border-radius: 8px;
      cursor: pointer;

      &.large {
        grid-column: span 7;
      }
      &:not(.large) {
        grid-column: span 5;
        margin-top: 10vw;
      }

      .image-wrapper {
        width: 100%;
        height: 100%;
        position: relative;

        img {
          width: 100%;
          height: 100%;
          object-fit: cover;
          transition: transform 0.7s cubic-bezier(0.25, 0.46, 0.45, 0.94);
        }

        .item-overlay {
          position: absolute;
          inset: 0;
          background: rgba(0,0,0,0.4);
          display: flex;
          flex-direction: column;
          justify-content: flex-end;
          padding: 2rem;
          opacity: 0;
          transition: opacity 0.4s ease;

          h3 {
            font-family: $font-display;
            font-size: 2rem;
            margin: 0 0 0.5rem;
          }
          p {
            margin: 0;
            font-size: 1rem;
            color: #ddd;
          }
        }
      }

      &:hover {
        .image-wrapper img {
          transform: scale(1.05);
        }
        .item-overlay {
          opacity: 1;
        }
      }
    }
  }
}

/* FOOTER */
.legal-footer {
  background: #050505;
  padding: 6rem 4rem 2rem;
  border-top: 1px solid rgba(255,255,255,0.1);

  .footer-grid {
    display: grid;
    grid-template-columns: 1fr 2fr 1fr;
    gap: 4rem;

    .footer-col {
      h4 {
        font-family: $font-display;
        font-size: 1.2rem;
        margin-bottom: 1.5rem;
        color: #fff;
        font-weight: 700;
      }
      p {
        color: $color-muted;
        font-size: 0.85rem;
        line-height: 1.6;
        margin-bottom: 0.5rem;
      }
      a {
        color: $color-muted;
        text-decoration: none;
        transition: color 0.3s;
        &:hover { color: $color-text; }
      }
    }

    .brand-col {
      .footer-logo {
        font-family: $font-display;
        font-size: 2rem;
        margin: 0 0 1rem;
      }
      .phones {
        font-size: 0.85rem;
        color: $color-muted;
        margin-bottom: 2rem;
      }
      .copyright {
        margin-top: 3rem;
        font-size: 0.75rem;
        opacity: 0.5;
      }
    }

    .legal-data {
      .data-grid {
        display: grid;
        grid-template-columns: 1fr 1fr;
        gap: 1.5rem 2rem;
        
        .data-item {
          display: flex;
          flex-direction: column;
          gap: 0.2rem;

          .label {
            font-size: 0.7rem;
            text-transform: uppercase;
            letter-spacing: 0.05em;
            color: #555;
          }
          .value {
            font-size: 0.85rem;
            color: #ccc;
          }
        }
      }
    }

    .address-col {
      .tax-tags {
        margin-top: 2rem;
        display: flex;
        flex-wrap: wrap;
        gap: 0.5rem;

        .tax-tag {
          font-size: 0.65rem;
          padding: 0.2rem 0.5rem;
          border: 1px solid #333;
          border-radius: 4px;
          color: #aaa;
        }
      }
    }
  }
}

/* ANIMATIONS */
@keyframes slowZoom {
  0% { transform: scale(1) translate(0, 0); }
  100% { transform: scale(1.1) translate(-2%, 2%); }
}
@keyframes revealUp {
  0% { transform: translateY(100%); opacity: 0; }
  100% { transform: translateY(0); opacity: 1; }
}
@keyframes fadeIn {
  to { opacity: 1; }
}
@keyframes scrollWheel {
  0% { transform: translate(-50%, 0); opacity: 1; }
  100% { transform: translate(-50%, 15px); opacity: 0; }
}
@keyframes marqueeMove {
  0% { transform: translateX(0); }
  100% { transform: translateX(-50%); }
}

/* RESPONSIVE */
@media (max-width: 1024px) {
  .hero { padding: 2rem; }
  .gallery { padding: 5vw 2rem; }
  .legal-footer .footer-grid {
    grid-template-columns: 1fr;
    gap: 3rem;
  }
  .gallery .gallery-grid {
    .gallery-item {
      &.large, &:not(.large) {
        grid-column: span 12;
        margin-top: 0;
      }
    }
  }
}
@media (max-width: 768px) {
  .legal-footer .legal-data .data-grid {
    grid-template-columns: 1fr;
  }
}
</style>

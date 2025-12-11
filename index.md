---
title: " "
layout: single
classes: wide home-wide
permalink: /
excerpt: "Ilustración, Concept Art y Modelado 3D con estética de fantasía oscura."
---

<div class="hero hero--dark-fantasy">
<img src= "/assets/images/LogoTituloWeb.png "
    alt="Logo Jose Velarde" 
    class="logo-hero"
    oncontextmenu="return false;" >

<p class="hero__subtitle">
Illustration · Concept Art · 3D Artist Junior.
</p>
</div>


<div class="home-hero-gallery">

  <figure class="home-hero-item">
    <img src="/PROYECTOS/INICIO/3D_1.png"
         alt="Habitación 3D y props para entorno interior">
  </figure>

  <figure class="home-hero-item">
    <img src="/PROYECTOS/INICIO/IlustracionAnime.png"
         alt="Ilustración de personaje con lobo de energía">
  </figure>  

  <figure class="home-hero-item">
    <img src="/PROYECTOS/INICIO/ilustracionCD.png"
         alt="Diseño gráfico de portada y CD">
  </figure>  

</div>




## About me

I'm a **Junior 3D Artist**, **Generalist**, and **Illustrator**.

My experience encompasses 3D modeling of props, environments, and characters, as well as 3D animation and game development in Unity. My specialty is **Anime-style Character Concept Art**, creating visual identities that work in both **comics** and **video games**.

I work with a balanced technical and aesthetic approach, paying close attention to every detail of the creative process: from concept design to final implementation. My goal is to deliver efficient, expressive, and tailored visual solutions for each project, creating experiences that stand out for their style and quality.

- I work from the initial idea to the final result: **3D modeling** of props, **environments, and characters**, **3D animation**, and **development in Unity**.

- I also have experience as an **illustrator for publishers**, developing images that narrate, complement, and enhance stories.

I always look to collaborate with studios, developers, or clients who value creativity, versatility, and visual innovation in their productions.





<div class="cv-wrapper">
  <img src="/assets/images/CVResumen.png"
       alt="Resumen CV de José Velarde"
       class="cv-image"
       oncontextmenu="return false;">
</div>

### Featured professional projects

- **3D rendered images for web pages** 
<div class="featured-projects">

  <article class="project-card">
    <figure class="project-thumb"
            data-full="PROYECTOS/3D/Molino1.png">
      <img src="PROYECTOS/3D/Molino1.png"
           alt="Título del proyecto 1">
    </figure>

    <p class="project-description">
      3D modeling of mechanical structures for website covers.
    </p>
  </article>
</div>



- **Educational 3D animations**

<div class="featured-projects">

  <article class="project-card project-card--video">
    <figure class="project-video-thumb"
            data-video="/PROYECTOS/3D/Animacion03.mp4">
      <img src="/PROYECTOS/3D/Animacion03.jpg"
           alt="Proyecto 2 – Vídeo demostración 1">
      <span class="video-thumb-play">▶</span>
    </figure>

    <p class="project-description">
      Animation to explain how a prototype machine works and what it is made of.
    </p>
  </article>

  <article class="project-card project-card--video">
    <figure class="project-video-thumb"
            data-video="/PROYECTOS/3D/Animacion_02.mp4">
      <img src="/PROYECTOS/3D/Animacion02.jpg"
           alt="Proyecto 2 – Vídeo demostración 2">
      <span class="video-thumb-play">▶</span>
    </figure>

    <p class="project-description">
      Explanatory animation about maintenance inside a wind turbine.
    </p>
  </article>

   <article class="project-card project-card--video">
    <figure class="project-video-thumb"
            data-video="/PROYECTOS/3D/Animacion_04.mp4">
      <img src="/PROYECTOS/3D/Animacion04.jpg"
           alt="Proyecto 2 – Vídeo demostración 3">
      <span class="video-thumb-play">▶</span>
    </figure>

    <p class="project-description">
      Explanatory animation about the function of a STATCOM Power Plant and its process.
    </p>
  </article>

</div>

- **Videogame Arcade (WEB Version)** 

<article class="project-card project-card--unity">
  <a href="https://josejvv.github.io/CelDamagePlanes/" 
     target="_blank" 
     rel="noopener noreferrer"
     class="project-unity-link">
    <figure class="project-video-thumb project-thumb-circle">
      <img src="/assets/images/MiniaturaJuego.png"
           alt="Cel Damage Planes">
    </figure>
  </a>

  <h3 class="project-title">Cel Damage Planes</h3>
  <p class="project-description">
    A game made entirely in Unity, based on the classic Space Shooter, transformed into an airplane version, where the objective is to destroy as many enemy planes as possible and score points. All programming and animation of the 3D models was done by me.
  </p>
</article>


<div class="image-lightbox" id="image-lightbox" aria-hidden="true">
  <div class="image-lightbox__backdrop"></div>

  <div class="image-lightbox__controls image-lightbox__controls--left">
    <button type="button"
            class="image-lightbox__btn image-lightbox__btn--fullscreen"
            aria-label="Ver a pantalla completa">⤢</button>
  </div>

  <div class="image-lightbox__controls image-lightbox__controls--right">
    <button type="button"
            class="image-lightbox__btn image-lightbox__btn--close"
            aria-label="Cerrar imagen">✕</button>
  </div>

  <img src="" alt="" id="image-lightbox-img">
</div>

<div class="video-lightbox" id="video-lightbox" aria-hidden="true">
  <div class="video-lightbox__backdrop"></div>

  <div class="video-lightbox__controls video-lightbox__controls--left">
    <button type="button"
            class="video-lightbox__btn video-lightbox__btn--fullscreen"
            aria-label="Ver a pantalla completa">⤢</button>
  </div>

  <div class="video-lightbox__controls video-lightbox__controls--right">
    <button type="button"
            class="video-lightbox__btn video-lightbox__btn--close"
            aria-label="Cerrar vídeo">✕</button>
  </div>

  <div class="video-lightbox__inner">
    <video id="video-lightbox-video" preload="metadata"></video>
    <div class="video-lightbox__pause-icon">⏸</div>
    <div class="video-lightbox__progress">
      <input type="range"
             id="video-progress"
             min="0"
             max="100"
             value="0"
             step="0.1">
    </div>
  </div>
</div>

<!-- SCRIPT ÚNICO: LIGHTBOX IMAGEN + VÍDEO -->
<script>
document.addEventListener("DOMContentLoaded", function () {
  /* === LIGHTBOX DE IMÁGENES (Proyecto 1) === */
  const imageLightbox = document.getElementById("image-lightbox");
  const imageLightboxImg = document.getElementById("image-lightbox-img");
  const imageBackdrop = imageLightbox?.querySelector(".image-lightbox__backdrop");
  const imageBtnClose = imageLightbox?.querySelector(".image-lightbox__btn--close");
  const imageBtnFullscreen = imageLightbox?.querySelector(".image-lightbox__btn--fullscreen");

  const imageThumbs = document.querySelectorAll(".project-thumb");

  if (imageLightbox && imageLightboxImg && imageBackdrop && imageBtnClose && imageBtnFullscreen) {
    imageThumbs.forEach(thumb => {
      thumb.addEventListener("click", () => {
        const fullSrc = thumb.getAttribute("data-full");
        const img = thumb.querySelector("img");
        const imgAlt = img ? img.getAttribute("alt") : "";
        if (!fullSrc) return;

        imageLightboxImg.src = fullSrc;
        imageLightboxImg.alt = imgAlt;
        imageLightbox.classList.add("is-active");
        document.body.style.overflow = "hidden";
      });
    });

    function closeImageLightbox() {
      imageLightbox.classList.remove("is-active");
      imageLightboxImg.src = "";
      document.body.style.overflow = "";
      if (document.fullscreenElement) {
        document.exitFullscreen().catch(() => {});
      }
    }

    imageBtnClose.addEventListener("click", closeImageLightbox);
    imageBackdrop.addEventListener("click", closeImageLightbox);

    document.addEventListener("keydown", (e) => {
      if (e.key === "Escape" && imageLightbox.classList.contains("is-active")) {
        closeImageLightbox();
      }
    });

    imageBtnFullscreen.addEventListener("click", () => {
      if (!document.fullscreenElement) {
        imageLightbox.requestFullscreen?.().catch(() => {});
      } else {
        document.exitFullscreen?.().catch(() => {});
      }
    });
  }

  /* === LIGHTBOX DE VÍDEO (SOLO TARJETAS DE VÍDEO, NO JUEGO) === */
  const videoThumbs = document.querySelectorAll(".project-card--video .project-video-thumb");
  const videoBox = document.getElementById("video-lightbox");
  const videoBackdrop = videoBox?.querySelector(".video-lightbox__backdrop");
  const videoEl = document.getElementById("video-lightbox-video");
  const videoBtnClose = videoBox?.querySelector(".video-lightbox__btn--close");
  const videoBtnFullscreen = videoBox?.querySelector(".video-lightbox__btn--fullscreen");
  const pauseIcon = videoBox?.querySelector(".video-lightbox__pause-icon");
  const videoProgress = document.getElementById("video-progress");

  if (videoBox && videoEl && videoBackdrop && videoBtnClose && videoBtnFullscreen && pauseIcon && videoProgress) {
    // Abrir y reproducir vídeo
    videoThumbs.forEach(thumb => {
      thumb.addEventListener("click", (e) => {
        const src = thumb.getAttribute("data-video");
        if (!src) return;       // si no hay data-video, no hace nada

        e.preventDefault();     // por si algún día hay <a> alrededor
        videoEl.src = src;
        videoBox.classList.add("is-active");
        document.body.style.overflow = "hidden";
        pauseIcon.style.display = "none";
        videoProgress.value = 0;

        videoEl.currentTime = 0;
        videoEl.play().catch(() => {});
      });
    });

    // Actualizar barra de progreso
    videoEl.addEventListener("timeupdate", () => {
      if (!videoEl.duration) return;
      const percentage = (videoEl.currentTime / videoEl.duration) * 100;
      videoProgress.value = percentage;
    });

    // Mover barra para avanzar/retroceder
    videoProgress.addEventListener("input", () => {
      if (!videoEl.duration) return;
      const newTime = (videoProgress.value / 100) * videoEl.duration;
      videoEl.currentTime = newTime;
    });

    // Pausar/Reanudar al hacer click en el vídeo
    videoEl.addEventListener("click", () => {
      if (videoEl.paused) {
        videoEl.play().catch(() => {});
        pauseIcon.style.display = "none";
      } else {
        videoEl.pause();
        pauseIcon.style.display = "flex";
      }
    });

    // Cerrar vídeo
    function closeVideoLightbox() {
      videoBox.classList.remove("is-active");
      videoEl.pause();
      videoEl.src = "";
      pauseIcon.style.display = "none";
      videoProgress.value = 0;
      document.body.style.overflow = "";
      if (document.fullscreenElement) {
        document.exitFullscreen().catch(() => {});
      }
    }

    videoBtnClose.addEventListener("click", closeVideoLightbox);
    videoBackdrop.addEventListener("click", closeVideoLightbox);

    document.addEventListener("keydown", (e) => {
      if (e.key === "Escape" && videoBox.classList.contains("is-active")) {
        closeVideoLightbox();
      }
    });

    // Pantalla completa
    videoBtnFullscreen.addEventListener("click", () => {
      if (!document.fullscreenElement) {
        videoBox.requestFullscreen?.().catch(() => {});
      } else {
        document.exitFullscreen?.().catch(() => {});
      }
    });
  }
});
</script>

<!-- SCRIPT ÚNICO PARA BLOQUEAR CLICK DERECHO EN IMÁGENES -->
<script>
document.addEventListener("contextmenu", function (e) {
  if (e.target && e.target.tagName === "IMG") {
    e.preventDefault();
  }
});
</script>

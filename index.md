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







## About me
I'm a **Junior 3D Artist**, **Generalist**, and **Illustrator**, and I'm passionate about bringing worlds to life. My specialty is **Anime-style Character Concept Art**, creating visual identities that work in both **comics** and **video games**.

- I work from the initial idea to the final result: **3D modeling** of props, **environments, and characters**, **3D animation**, and **development in Unity**.

- I also have experience as an **illustrator for publishers**, developing images that narrate, complement, and enhance stories.

My goal is to transform each concept into something that inspires, excites, and connects, turning imagination into real visual experiences.





<div class="cv-wrapper">
  <img src="/assets/images/CVResumen.png"
       alt="Resumen CV de José Velarde"
       class="cv-image"
       oncontextmenu="return false;">
</div>

### Featured professional projects

- **Imagenes renderizadas 3D para paginas Web** 
<div class="featured-projects">

  <article class="project-card">
    <figure class="project-thumb"
            data-full="PROYECTOS/3D/Molino1.png">
      <img src="PROYECTOS/3D/Molino1.png"
           alt="Título del proyecto 1">
    </figure>

    <p class="project-description">
      Modelado 3D de estructuras mecánicas para portadas de pàginas web.
    </p>
  </article>
</div>



- **Animaciones 3D educativas**

<div class="featured-projects">

  <article class="project-card project-card--video">
    <figure class="project-video-thumb"
            data-video="/PROYECTOS/3D/Animacion03.mp4">
      <img src="/PROYECTOS/3D/Animacion03.jpg"
           alt="Proyecto 2 – Vídeo demostración 1">
      <span class="video-thumb-play">▶</span>
    </figure>

    <p class="project-description">
      Breve descripción del vídeo: objetivo, tipo de proyecto, software usado, etc.
    </p>
  </article>

  <article class="project-card project-card--video">
    <figure class="project-video-thumb"
            data-video="/PROYECTOS/3D/Animacion_02.mp4">
      <img src="/PROYECTOS/3D/Animacion_02.png"
           alt="Proyecto 2 – Vídeo demostración 2">
      <span class="video-thumb-play">▶</span>
    </figure>

    <p class="project-description">
      Breve descripción del vídeo: objetivo, tipo de proyecto, software usado, etc.
    </p>
  </article>

   <article class="project-card project-card--video">
    <figure class="project-video-thumb"
            data-video="/PROYECTOS/3D/Animacion_04.mp4">
      <img src="/PROYECTOS/3D/Animacion_04.png"
           alt="Proyecto 2 – Vídeo demostración 3">
      <span class="video-thumb-play">▶</span>
    </figure>

    <p class="project-description">
      Breve descripción del vídeo: objetivo, tipo de proyecto, software usado, etc.
    </p>
  </article>

</div>

- **[Proyecto 3]** – Técnicas y herramientas utilizadas.
Puedes detallar estos proyectos más adelante dentro de las secciones de **Ilustración** y **3D**.




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
  </div>
</div>

<script>
document.addEventListener("DOMContentLoaded", function () {
  /* === LIGHTBOX DE IMAGEN (ya lo tenías) === */
  const thumbs = document.querySelectorAll(".project-thumb");
  const lightbox = document.getElementById("image-lightbox");
  const lightboxImg = document.getElementById("image-lightbox-img");
  const backdrop = lightbox?.querySelector(".image-lightbox__backdrop");
  const btnClose = lightbox?.querySelector(".image-lightbox__btn--close");
  const btnFullscreen = lightbox?.querySelector(".image-lightbox__btn--fullscreen");

  if (lightbox && lightboxImg && backdrop && btnClose && btnFullscreen) {
    thumbs.forEach(thumb => {
      thumb.addEventListener("click", () => {
        const fullSrc = thumb.getAttribute("data-full");
        const img = thumb.querySelector("img");
        const imgAlt = img ? img.getAttribute("alt") : "";
        lightboxImg.src = fullSrc;
        lightboxImg.alt = imgAlt;
        lightbox.classList.add("is-active");
        document.body.style.overflow = "hidden";
      });
    });

    function closeImageLightbox() {
      lightbox.classList.remove("is-active");
      lightboxImg.src = "";
      document.body.style.overflow = "";
      if (document.fullscreenElement) {
        document.exitFullscreen().catch(() => {});
      }
    }

    btnClose.addEventListener("click", closeImageLightbox);
    backdrop.addEventListener("click", closeImageLightbox);

    document.addEventListener("keydown", (e) => {
      if (e.key === "Escape" && lightbox.classList.contains("is-active")) {
        closeImageLightbox();
      }
    });

    btnFullscreen.addEventListener("click", () => {
      if (!document.fullscreenElement) {
        lightbox.requestFullscreen?.().catch(() => {});
      } else {
        document.exitFullscreen?.().catch(() => {});
      }
    });
  }

  /* === LIGHTBOX DE VÍDEO === */
  const videoThumbs = document.querySelectorAll(".project-video-thumb");
  const videoBox = document.getElementById("video-lightbox");
  const videoBackdrop = videoBox?.querySelector(".video-lightbox__backdrop");
  const videoEl = document.getElementById("video-lightbox-video");
  const videoBtnClose = videoBox?.querySelector(".video-lightbox__btn--close");
  const videoBtnFullscreen = videoBox?.querySelector(".video-lightbox__btn--fullscreen");
  const pauseIcon = videoBox?.querySelector(".video-lightbox__pause-icon");

  if (videoBox && videoEl && videoBackdrop && videoBtnClose && videoBtnFullscreen && pauseIcon) {
    // Abrir y reproducir vídeo
    videoThumbs.forEach(thumb => {
      thumb.addEventListener("click", () => {
        const src = thumb.getAttribute("data-video");
        videoEl.src = src;
        videoBox.classList.add("is-active");
        document.body.style.overflow = "hidden";
        pauseIcon.style.display = "none";

        videoEl.currentTime = 0;
        videoEl.play().catch(() => {});
      });
    });

    // Pausar / reanudar al hacer click sobre el vídeo
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


<script>
document.addEventListener("contextmenu", function(e) {
  if (e.target.tagName === "IMG") {
    e.preventDefault();
  }
});
</script>

<script>
document.addEventListener("contextmenu", function (e) {
  if (e.target && e.target.tagName === "IMG") {
    e.preventDefault();
  }
});
</script>
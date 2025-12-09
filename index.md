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

### Proyectos profesionales destacados

- **[Proyecto 1]** – Breve descripción del proyecto, cliente o estudio, y tu rol principal.
<div class="featured-projects">

  <article class="project-card">
    <figure class="project-thumb"
            data-full="PROYECTOS/3D/Molino1.png">
      <img src="PROYECTOS/3D/Molino1.png"
           alt="Título del proyecto 1">
    </figure>

    <h3 class="project-title">Proyecto 1 – Solute1</h3>
    <p class="project-description">
      Breve descripción del proyecto, cliente o propósito del arte.
    </p>
  </article>

</div>



- **[Proyecto 2]** – Qué resolviste visualmente (diseño de personajes, entornos, props…).
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

<script>
document.addEventListener("DOMContentLoaded", function () {
  const thumbs = document.querySelectorAll(".project-thumb");
  const lightbox = document.getElementById("image-lightbox");
  const lightboxImg = document.getElementById("image-lightbox-img");
  const backdrop = lightbox.querySelector(".image-lightbox__backdrop");
  const btnClose = lightbox.querySelector(".image-lightbox__btn--close");
  const btnFullscreen = lightbox.querySelector(".image-lightbox__btn--fullscreen");

  // Abrir lightbox al hacer click en miniatura
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

  // Cerrar lightbox
  function closeLightbox() {
    lightbox.classList.remove("is-active");
    document.body.style.overflow = "";
    if (document.fullscreenElement) {
      document.exitFullscreen().catch(() => {});
    }
  }

  btnClose.addEventListener("click", closeLightbox);
  backdrop.addEventListener("click", closeLightbox);

  // Cerrar con la tecla ESC
  document.addEventListener("keydown", (e) => {
    if (e.key === "Escape" && lightbox.classList.contains("is-active")) {
      closeLightbox();
    }
  });

  // Pantalla completa
  btnFullscreen.addEventListener("click", () => {
    if (!document.fullscreenElement) {
      if (lightbox.requestFullscreen) {
        lightbox.requestFullscreen().catch(() => {});
      }
    } else {
      document.exitFullscreen?.().catch(() => {});
    }
  });
});
</script>


<script>
document.addEventListener("contextmenu", function(e) {
  if (e.target.tagName === "IMG") {
    e.preventDefault();
  }
});
</script>
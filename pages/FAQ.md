---
layout: default
title: FAQ
permalink: "/faq/"
---

<h1>Preguntas Frecuentes</h1>

<div class="acordeon-container">
  <div class="acordeon-item">
    <button class="acordeon-question">¿Qué es Permaprendices?</button>
    <div class="acordeon-answer">
      <p>Es un proyecto donde compartimos experiencias, aprendizajes y aventuras relacionados con la permacultura, la sintrópica y la vida en comunidad.</p>
    </div>
  </div>

  <div class="acordeon-item">
    <button class="acordeon-question">¿Quiénes sois?</button>
    <div class="acordeon-answer">
      <p>Somos Andreu y Marta, dos exploradores del decrecimiento con alma de huerto y corazón nómada.</p>
    </div>
  </div>

  <div class="acordeon-item">
    <button class="acordeon-question">¿Cómo puedo colaborar?</button>
    <div class="acordeon-answer">
      <p>Puedes unirte como voluntario, compartir nuestros artículos o simplemente escribirnos para echar un rato bonito.</p>
    </div>
  </div>
</div>

<script>
  document.addEventListener("DOMContentLoaded", function () {
    const questions = document.querySelectorAll(".acordeon-question");

    questions.forEach(button => {
      button.addEventListener("click", () => {
        const answer = button.nextElementSibling;
        const expanded = button.getAttribute("aria-expanded") === "true";
        
        button.setAttribute("aria-expanded", !expanded);
        answer.style.maxHeight = !expanded ? answer.scrollHeight + "px" : null;
      });
    });
  });
</script>

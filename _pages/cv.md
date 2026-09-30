---
layout: cv
permalink: /cv/
title: CV
nav: true
nav_order: 5
cv_format: rendercv
description: Academic curriculum vitae highlighting my research, teaching, and scientific experience in physics, plasmonics, SERS, nanophotonics, and optical spectroscopy.
toc:
  sidebar: left
---

<style>
  /* Correo institucional con el mismo magenta del sitio */
  .cv-email-custom {
    color: var(--global-theme-color) !important;
    text-decoration: none !important;
  }

  .cv-email-custom:hover {
    text-decoration: underline !important;
  }
</style>

<script>
document.addEventListener("DOMContentLoaded", function () {

  const email = "luisguerra@unipamplona.edu.co";
  const address =
    "Universidad de Pamplona, Km 1 vía Bucaramanga, Pamplona, Norte de Santander, Colombia";

  /* ------------------------------------------------------
     1. Localizar únicamente la tarjeta Contact Information
     ------------------------------------------------------ */

  const headings = Array.from(
    document.querySelectorAll("h1, h2, h3, h4, h5")
  );

  const contactHeading = headings.find(
    el => el.textContent.trim() === "Contact Information"
  );

  if (!contactHeading) return;

  const contactCard =
    contactHeading.closest(".card") ||
    contactHeading.parentElement;

  if (!contactCard) return;


  /* ------------------------------------------------------
     2. Convertir el correo en enlace y darle color magenta
     ------------------------------------------------------ */

  const elements = Array.from(
    contactCard.querySelectorAll("a, span, div, p, td, dd")
  );

  const emailElement = elements.find(
    el =>
      el.children.length === 0 &&
      el.textContent.trim() === email
  );

  if (emailElement) {

    if (emailElement.tagName.toLowerCase() === "a") {

      emailElement.href = "mailto:" + email;
      emailElement.classList.add("cv-email-custom");

    } else {

      const link = document.createElement("a");
      link.href = "mailto:" + email;
      link.textContent = email;
      link.className = "cv-email-custom";

      emailElement.textContent = "";
      emailElement.appendChild(link);
    }
  }


  /* ------------------------------------------------------
     3. Copiar exactamente el formato de la fila Email
        para crear Institutional Address
     ------------------------------------------------------ */

  const allElements = Array.from(contactCard.querySelectorAll("*"));

  const emailLabel = allElements.find(
    el =>
      el.children.length === 0 &&
      el.textContent.trim() === "Email"
  );

  if (!emailLabel) return;

  let emailRow = emailLabel;

  while (emailRow && emailRow !== contactCard) {

    const text = emailRow.textContent
      .replace(/\s+/g, " ")
      .trim();

    if (text.includes("Email") && text.includes(email)) {
      break;
    }

    emailRow = emailRow.parentElement;
  }

  if (!emailRow || emailRow === contactCard) return;

  /* Evitar duplicados */
  if (contactCard.textContent.includes(address)) return;

  const addressRow = emailRow.cloneNode(true);

  const addressElements = Array.from(
    addressRow.querySelectorAll("*")
  );

  const clonedLabel = addressElements.find(
    el =>
      el.children.length === 0 &&
      el.textContent.trim() === "Email"
  );

  if (clonedLabel) {
    clonedLabel.textContent = "Institutional Address";
  }

  const clonedEmail = addressElements.find(
    el =>
      el.children.length === 0 &&
      el.textContent.trim() === email
  );

  if (clonedEmail) {

    if (clonedEmail.tagName.toLowerCase() === "a") {
      clonedEmail.removeAttribute("href");
      clonedEmail.classList.remove("cv-email-custom");
    }

    clonedEmail.textContent = address;
  }

  emailRow.insertAdjacentElement("afterend", addressRow);

});
</script>

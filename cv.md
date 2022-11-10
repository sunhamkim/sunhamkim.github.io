---
layout: homepage
---

You can download my CV [here](https://sunhamkim.github.io/files/pdf/CurriculumVitae_SKim.pdf){:target="_blank" rel="noopener"}. [[back](./)]

<style>
/* Only resize the element if PDF is embedded */
.pdfobject-container {
   width: 450px;
   height: 400px;
}
</style>

<div id="my-pdf"></div>

<script src="https://sunhamkim.github.io/assets/js/pdfobject.js"></script>

<script>
  var options = {
     width: "40rem",
     height: "35rem",
     fallbackLink: false
  };
  PDFObject.embed("https://sunhamkim.github.io/files/pdf/CurriculumVitae_SKim.pdf", "#my-pdf", options);
</script>

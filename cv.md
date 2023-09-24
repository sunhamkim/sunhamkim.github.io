---
layout: homepage
---
<div class="blank-div"></div>
You can download my CV [here](https://sunhamkim.github.io/files/pdf/CurriculumVitae_SKim.pdf){:target="_blank" rel="noopener"}. 

<style>
/* Only resize the element if PDF is embedded */
.pdfobject-container {
   width: 480px;
   height: 600px;
}
</style>

<div id="my-pdf"></div>

<script src="./assets/js/pdfobject.js" type="text/javascript"></script>
<script>
  var options = {
     width: "40rem",
     height: "35rem",
     fallbackLink: false
  };
  PDFObject.embed("https://sunhamkim.github.io/files/pdf/CurriculumVitae_SKim.pdf", "#my-pdf", options);
</script>

<a href="./" class="btn btn-sm z-depth-0" role="button" style="font-size:12px; color: #000000; border: 1px solid #000000; padding-left: 0.5rem; padding-right: 0.5rem; padding-top: 0.1rem; padding-bottom: 0.1rem;;">Back</a>
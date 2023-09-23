<h1 id="ongoing"></h1>

<h2 style="margin: 0px 0px -15px;">Working Papers</h2>


<div class="publications">
<ol class="bibliography">

{% for link in site.data.ongoing.main %}

<li>
<div class="pub-row">
  <div class="col-sm-12" style="position: relative;padding-right: 15px;padding-left: 20px;">
      <div class="title">{{ link.title }}</div>
      <div class="author" style="display: inline;">{{ link.authors }}</div>
      {% if link.status %}
      <span class="periodical"><em>{{ link.status }}</em></span>
      {% endif %}
      {% if link.media %} 
      <div class="media">{{ link.media }}</div>
      {% endif %}
    <div class="links">
      {% if link.pdf %} 
      <a href="{{ link.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Draft</a>
      {% endif %}
      {% if link.abstract %} 
      <a href="#" class="btn btn-sm z-depth-0 abstract-toggle-button" role="button" style="font-size:12px;" onclick="event.preventDefault(); toggleAbstract(this);">Abstract</a>
      {% endif %}
      {% if link.code %} 
      <a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Code</a>
      {% endif %}
      {% if link.page %} 
      <a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Project Page</a>
      {% endif %}
      {% if link.bibtex %} 
      <a href="{{ link.bibtex }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">BibTex</a>
      {% endif %}
      {% if link.notes %} 
      <strong> <i style="color:#e74d3c">{{ link.notes }}</i></strong>
      {% endif %}
      {% if link.others %} 
      {{ link.others }}
      {% endif %}
    </div>
      {% if link.abstract %}
      <div class="abstract-content col-sm-12" style="display: none;">
        {{ link.abstract }}
      </div>
      {% endif %}
  </div>
</div>
</li>

{% endfor %}

</ol>
</div>

<script>
  function toggleAbstract(button) {
      console.log('toggleAbstract function triggered!');
      console.log('Clicked button:', button);

      // Go up to the parent div (class: col-sm-12)
      var parentDiv = button.closest('.col-sm-12');

      if (parentDiv) {
          // Find the child element with class abstract-content
          var abstractContent = parentDiv.querySelector('.abstract-content');
          
          if (abstractContent) {
              console.log('Found abstractContent:', abstractContent);
              abstractContent.style.display = (abstractContent.style.display === 'none') ? '' : 'none';
          } else {
              console.error('abstractContent is null. Check the HTML structure.');
          }
      } else {
          console.error('Parent div (col-sm-12) not found. Check the HTML structure.');
      }
  }
</script>
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
      <button class="btn btn-sm z-depth-0 abstract-toggle-button" style="font-size:12px;">Abstract</button>
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
      {% if link.abstract%}
      <div class="abstract-content col-sm-12" style="display: none;">
      </div>
      {% endif %}
  </div>
</div>
</li>

{% endfor %}
      

</ol>
</div>

<script>
  document.querySelectorAll('.abstract-toggle-button').forEach(function(button) {
    button.addEventListener('click', function() {
      var abstractContent = button.nextElementSibling;
      abstractContent.style.display = (abstractContent.style.display === 'none') ? '' : 'none';
    });
  });
</script>
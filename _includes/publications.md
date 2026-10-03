<h2 id="publications" style="margin: 0px 0px -15px;">Publications</h2>

<div class="publications">
<ol class="bibliography">

{% for link in site.data.publications.main %}

<li>
<div class="pub-row">
  <div class="col-sm-12" style="position: relative;padding-right: 15px;padding-left: 20px;">
      <div class="title">{{ link.title }}</div>
      {% if link.authors %}
      <div class="author" style="display: inline;">{{ link.authors }}</div>
      {% endif %}
      {% if link.oldtitle %}
      <span class="oldtitle">{% if link.authors %}<br>{% endif %}previously, <i>{{ link.oldtitle }}</i></span>
      {% endif %}
      <span class="periodical">{% if link.authors or link.oldtitle %}<br>{% endif %}<em><strong style="color:var(--global-theme-color); font-weight:600">{{ link.journal }}</strong>, {{ link.status }}{% if link.date and link.date != empty %}, {{ link.date | append: "" | slice: 0, 4 }}{% endif %}</em></span>
      {% if link.media %} 
      <div class="media">{{ link.media }}</div>
      {% endif %}
    <div class="links">
      {% if link.abstract %} 
      <a href="#" class="btn btn-sm z-depth-0 abstract-toggle-button" role="button" style="font-size:12px;" onclick="event.preventDefault(); toggleAbstract(this);">Abstract</a>
      {% endif %}
      {% if link.pdf %} 
      <a href="{{ link.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank" rel="noopener" style="font-size:12px;">WP version</a>
      {% endif %}
      {% if link.journal_url and link.journal_url != empty %}
      <a href="{{ link.journal_url }}" class="btn btn-sm z-depth-0" role="button" target="_blank" rel="noopener" style="font-size:12px;">Published version</a>
      {% endif %}
      {% if link.youtube %}
      <a href="{{ link.youtube }}" class="btn btn-sm z-depth-0" role="button" target="_blank" rel="noopener" style="font-size:12px;">YouTube</a>
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
      <div class="abstract-content col-sm-12" style="display: none; margin-top: 10px; margin-left: 0px; margin-right: 15px; margin-bottom: 10px;">
        {{ link.abstract }}
      </div>
      {% endif %}
  </div>
</div>
</li>

{% endfor %}

</ol>
</div>

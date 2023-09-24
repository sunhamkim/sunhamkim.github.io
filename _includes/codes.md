<h1 id="codes"></h1>

<h2 style="margin: 0px 0px -15px;">Codes</h2>
<div class="publications">
<ol class="bibliography">

{% for link in site.data.codes.main %}

<li>
<div class="pub-row">
  <div class="col-sm-12" style="position: relative;padding-right: 15px;padding-left: 20px;">
      <div class="title">{{ link.title }}</div>
      <div class="author" style="display: inline;">{{ link.authors }} </div>
    <div class="links">
      {% if link.notes %} 
        {{ link.notes }} <br>
      {% endif %}  
      {% if link.code %} 
      <a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Code</a>
      {% endif %}
      {% if link.others %} 
        {{ link.others }}
      {% endif %}
    </div>
  </div>
</div>
</li>

{% endfor %}

</ol>
</div>

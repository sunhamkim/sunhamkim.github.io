<h1 id="policy"></h1>

<h2 style="margin: 0px 0px 10px;">
  Policy Work
  <a href="#" class="btn btn-sm z-depth-0 custom-toggle-button" role="button" onclick="event.preventDefault(); toggleSection(this, 'policy-content');">
    Expand
  </a>
</h2>

<div id="policy-content" style="display:none;">
<div class="publications">
<ol class="bibliography">

{% for item in site.data.policy.main %}
<li>
<div class="pub-row">
  <div class="col-sm-12" style="position: relative; padding-right: 15px; padding-left: 20px;">
    <div class="title"><span lang="ko">{{ item.title }}</span></div>
    {% if item.authors %}
    <div class="author" style="display: inline;">{{ item.authors }}</div>
    {% endif %}
    {% if item.series or item.date %}
    <span class="periodical">{% if item.authors %}<br>{% endif %}{% if item.series %}<em lang="ko">{{ item.series }}</em>{% endif %}{% if item.series and item.date %}, {% endif %}{% if item.date %}{{ item.date }}{% endif %}</span>
    {% endif %}
    <div class="links">
      {% if item.abstract %}
      <a href="#" class="btn btn-sm z-depth-0 abstract-toggle-button" role="button" style="font-size:12px;" onclick="event.preventDefault(); toggleAbstract(this);">Abstract</a>
      {% endif %}
      {% if item.pdf %}
      <a href="{{ item.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank" rel="noopener" style="font-size:12px;">PDF</a>
      {% endif %}
      {% if item.notes %}
      <strong><i lang="ko" style="color:#e74d3c">{{ item.notes }}</i></strong>
      {% endif %}
    </div>
    {% if item.abstract %}
    <div class="abstract-content col-sm-12" style="display: none; margin-top: 10px; margin-left: 0px; margin-right: 15px; margin-bottom: 10px;">
      <span lang="ko">{{ item.abstract }}</span>
    </div>
    {% endif %}
  </div>
</div>
</li>
{% endfor %}

</ol>
</div>
</div>

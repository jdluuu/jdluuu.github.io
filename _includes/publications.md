<h2 id="publications" style="margin: 2px 0px -15px;">Publications</h2>

<div class="publications">
<ol class="bibliography">

{% for link in site.data.publications.main %}

<li>
<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    {% if link.image %}
    {% if link.details %}
    <a href="#" class="project-modal-trigger" data-project-id="pub-{{ forloop.index }}"><img src="{{ link.image }}" class="teaser img-fluid z-depth-1" style="width=100;height=40%"></a>
    {% else %}
    <img src="{{ link.image }}" class="teaser img-fluid z-depth-1" style="width=100;height=40%">
    {% endif %}
    {% if link.conference_short %}
    <abbr class="badge">{{ link.conference_short }}</abbr>
    {% endif %}
    {% endif %}
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
      <div class="title">
        {% if link.details %}
        <a href="#" class="project-modal-trigger" data-project-id="pub-{{ forloop.index }}">{{ link.title }}</a>
        {% else %}
        <a href="{{ link.pdf }}">{{ link.title }}</a>
        {% endif %}
      </div>
      {% if link.details %}
      <template id="pub-{{ forloop.index }}-content">
        <h2 class="modal-title">{{ link.title }}</h2>
        {% if link.details.images_first %}
        {% for img in link.details.images %}
        <figure class="modal-figure">
          <img src="{{ img.url }}" alt="{{ img.caption }}">
          {% if img.caption %}<figcaption>{{ img.caption }}</figcaption>{% endif %}
        </figure>
        {% endfor %}
        {% endif %}
        {% if link.details.description %}
        <div class="modal-description">{{ link.details.description }}</div>
        {% endif %}
        {% unless link.details.images_first %}
        {% for img in link.details.images %}
        <figure class="modal-figure">
          <img src="{{ img.url }}" alt="{{ img.caption }}">
          {% if img.caption %}<figcaption>{{ img.caption }}</figcaption>{% endif %}
        </figure>
        {% endfor %}
        {% endunless %}
        {% for vid in link.details.videos %}
        <figure class="modal-figure">
          <iframe src="{{ vid.url }}" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
          {% if vid.caption %}<figcaption>{{ vid.caption }}</figcaption>{% endif %}
        </figure>
        {% endfor %}
      </template>
      {% endif %}
      <div class="author">{{ link.authors }}</div>
      <div class="periodical"><em>{{ link.conference }}</em>
      </div>
    <div class="links">
      {% if link.pdf %}
      <a href="{{ link.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
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
    </div>
    <div class="notes">
      {% if link.notes %}
      <strong> <i style="color:#e74d3c">{{ link.notes }}</i></strong>
      {% endif %}
    </div>
    <div class="others">
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

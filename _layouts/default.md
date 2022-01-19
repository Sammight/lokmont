<!DOCTYPE html>
<html lang="en">

  {% include head.md %}
  
  {% if page.url == '/' %}
    {% assign class = 'body-post' %}
  <body class="{{ class }}">
  {% endif %}
  
    {% if site.google-analytics %}
      {% include google-analytics.html %}
    {% endif %}

    <div class="full-page-container">
      <div class="overlay"></div>
      {% include header.md %}
      {% include search.md %}

        {{ content }}

      {% include scroll-top.md %}
      {% include footer.md %}
    </div> <!-- /.full-page-container -->

    {% include javascripts.md %}
  </body>

</html>

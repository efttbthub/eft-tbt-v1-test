
{% capture sidebar %}{% include ajeter.md %}{% endcapture %}
{{ sidebar | markdownify }}

{% markdown 020-presentation.md %}



{% for year in (1983..2013) %}
  {% capture filename %}../alumni/{{year}}.html{% endcapture %}
  {% include {{filename}} %}
{% endfor %}
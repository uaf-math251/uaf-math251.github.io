---
layout: course-page
title: Worksheets
---

### In-person Worksheets

<div class="x-scroll">
<table class="asst-table">
<tr><th>Section</th><th>Topic</th><th>Materials</th></tr>
{% for c in site.data.ipworksheets-f2024 %}
<tr valign="top">
  <td>
    {{ c.name }}
  </td>
  <td>
    {{ c.topic }}
  </td>
  <td>
    <table class="inner">
      <tr>
         <td> <a href="{{ c.urlblank }}">blank</a> </td>
      </tr>
      {% if c.urlfilled %}
      <tr>
         <td> <a href="{{ c.urlfilled }}">filled</a> </td>
      </tr>
      {% endif %}
      {% if c.urlvideo1 %}
      <tr>
         <td> <a href="{{ c.urlvideo1 }}">video 1 </a><br></td>         
      </tr>
      {% endif %}
      {% if c.urlvideo2 %}
       <tr>
         <td> <a href="{{ c.urlvideo2 }}">video 2 </a><br></td>         
      </tr>
      {% endif %}
    </table>
  </td>
</tr>
{% endfor %}
</table>
</div>

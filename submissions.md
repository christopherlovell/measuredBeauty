---
layout: page
title: Submissions
permalink: /submissions/
---

Submissions to *Measured Beauty* are welcome. Please follow these guidelines when preparing your submission, then use the form below to express your interest and idea. I reserve editorial discretion.

- The original data should be from real world observations. Plots based on simulation data are not currently accepted.
- 'Cleaned' images should, where possible, have no axis, labels or surrounding text.
- Both the original as well as the 'cleaned' image must be submitted.
- Submissions including a short (max. 500 words) lay-mans description of what the plot shows will be prioritised.
- Authors of papers with higher resolution original images available are encouraged to submit these rather than screen grabs from papers.


<div class="py2">
  {% if site.ajaxify_contact_form %}
    <form class="form-stacked">
      <input type="text" name="email" class="field-light" placeholder="Email Address">
      <textarea type="text" name="content" class="field-light" rows="5" placeholder="What would you like to say?"></textarea>
      <input type="hidden" name="_subject" value="New submission!" />
      <input type="text" name="_gotcha" style="display:none" />
      <button type='submit' class="button button-blue button-big mobile-block">Say Hello</button>
    </form>
  {% else %}
    <form action="https://formspree.io/{{ site.email }}" method="POST" class="form-stacked">
      <input type="text" name="email" class="field-light" placeholder="Email Address">
      <textarea type="text" name="content" class="field-light" rows="5" placeholder="What would you like to say?"></textarea>
      <input type="hidden" name="_next" value="{{ site.baseurl }}/thanks/" />
      <input type="hidden" name="_subject" value="New submission!" />
      <input type="text" name="_gotcha" style="display:none" />
      <input type="submit" class="button button-blue button-big mobile-block" value="Say Hello">
    </form>
  {% endif %}
</div>

{% if site.ajaxify_contact_form %}
  {% include ajaxify_content_form.html %}
{% endif %}

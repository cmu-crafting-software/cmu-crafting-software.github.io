---
layout: page
title: Assignments
description: Listing of course assignments.
---

# Assignments

{% for assignments in site.assignments %}
{{ assignment }}
{% endfor %}

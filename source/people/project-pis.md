---
layout: default
title: NYU DH Project PIs
breadcrumbs:
  - name: People
    link: /people
contents_links:
    - label: 'NYU DH Faculty Seed Grant Program'
      link: '/funding/seed-grants/'
    - label: 'View All Projects'
      link: '/projects'
---
{% assign people = site.data.people | where_exp: "p", "p.site_roles contains 'proj_pi'" %}
{% assign people = people | sort: 'pid' %}
{% include custom/people-cards.html data=people full_width=false %}
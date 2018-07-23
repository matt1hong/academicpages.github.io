---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* M.S. Computer Science, **Northwestern University**, 2016
  * Specialization: Human-Computer Interaction
  * Advisors: Oliver Cossairt, Michael Horn
* B.A. Mathematics, **Northwestern University**, 2016
  * Specialization: Probability Theory
  * Advisors: Michael Stein, Steven Franconeri
* Study Abroad, **University of Southampton**, 2013
  * Specialization: Medieval Archaeology
  * Advisor: Matthew H. Johnson
* Qualified Associate Certification, **Tableau Software**

Research positions
======
* **Visual Thinking Lab**, PI: Steven Franconeri
  * 2013-16

* **Knight Lab**, PI: Rich Gordon
  * 2014-15

* **Amaral Lab**, PI: Luis Amaral
  * 2012-13
  
Skills
======
* _Programming_: Python (Flask, data analytics), JavaScript (React.js, Node.js, D3.js), HTML, CSS, C#, Java
* _Design_: Adobe Photoshop, Illustrator, InDesign, Tableau

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Teaching
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}
  </ul>
  <ul>{% for post in site.talks reversed %}
    {% include archive-single-talk-cv.html %}
  {% endfor %}</ul>
  
Employment
======
* Full-stack Software Engineer, **My.Suit**
  * 2016-2017
* Data Visualization Developer, **Blackstone Market Research**
  * 2016
* Design Editor, **The Daily Northwestern**
  * 2012

---
layout: workshop      # DON'T CHANGE THIS.
# More detailed instructions (including how to fill these variables for an
# online workshop) are available at
# https://carpentries.github.io/workshop-template/customization/index.html
venue: "csv,conf,v8 - Benemérita Universidad Autónoma de Puebla (BUAP)"        # brief name of the institution that hosts the workshop without address (e.g., "Euphoric State University")
address: "Benemérita Universidad Autónoma de Puebla (BUAP) Heroica Puebla de Zaragoza Puebla, PUE 72592 Mexico"      # full street address of workshop (e.g., "Room A, 123 Forth Street, Blimingen, Euphoria"), videoconferencing URL, or 'online'
country: "Mexico"      # lowercase two-letter ISO country code such as "fr" (see https://en.wikipedia.org/wiki/ISO_3166-1#Current_codes) for the institution that hosts the workshop
language: "es"     # lowercase two-letter ISO language code such as "fr" (see https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) for the workshop
latitude: "19.00200"        # decimal latitude of workshop venue (use https://www.latlong.net/)
longitude: "-98.19991"       # decimal longitude of the workshop venue (use https://www.latlong.net)
humandate: "May 27-28, 2024"    # human-readable dates for the workshop (e.g., "Feb 17-18, 2020")
humantime: "9:00 am - 4:30 pm"    # human-readable times for the workshop e.g., "9:00 am - 4:30 pm CEST (7:00 am - 2:30 pm UTC)"
startdate: 2024-05-27      # machine-readable start date for the workshop in YYYY-MM-DD format like 2015-01-01
enddate: 2024-05-28        # machine-readable end date for the workshop in YYYY-MM-DD format like 2015-01-02
instructor: ["Gabriel Alarcón Carranza", "Shaday Guerrero Flores"] # boxed, comma-separated list of instructors' names as strings, like ["Kay McNulty", "Betty Jennings", "Betty Snyder"]
helper: ["Heladia Salgado", "Haydeé Contreras Peruyero", "Evelia Coss Navarrete"]     # boxed, comma-separated list of helpers' names, like ["Marlyn Wescoff", "Fran Bilas", "Ruth Lichterman"]
email: ["helysalgado@gmail.com","shaday@matmor.unam.mx", "alarcongabriel128@gmail.com","ecoss@liigh.unam.mx","haydeeperuyero@matmor.unam.mx"]    # boxed, comma-separated list of contact email addresses for the host, lead instructor, or whoever else is handling questions, like ["marlyn.wescoff@example.org", "fran.bilas@example.org", "ruth.lichterman@example.org"]
collaborative_notes: https://docs.google.com/document/d/1aL570D2lqN_0bHSR9s-EDkNjowodZGRDmR4e71YvqnY/edit?usp=sharing # https://pad.carpentries.org/2024-05-27-csvconf  # optional: URL for the workshop collaborative notes, e.g. an Etherpad or Google Docs document (e.g., https://pad.carpentries.org/2015-01-01-euphoria)

---
{% comment %} See instructions in the comments below for how to edit specific sections of this workshop template. {% endcomment %}

{% comment %}
HEADER

Edit the values in the block above to be appropriate for your workshop.
If the value is not 'true', 'false', 'null', or a number, please use
double quotation marks around the value, unless specified otherwise.
And run 'make workshop-check' *before* committing to make sure that changes are good.
{% endcomment %}


{% comment %}

{% endcomment %}


{% comment %}
Check DC curriculum
{% endcomment %}

{% if site.carpentry == "dc" %}
{% unless site.curriculum == "dc-astronomy" or site.curriculum == "dc-ecology" or site.curriculum == "dc-genomics" or site.curriculum == "dc-geospatial" or site.curriculum == "dc-image" or site.curriculum == "dc-socsci" %}
<div class="alert alert-warning">
It looks like you are setting up a website for a Data Carpentry curriculum but you haven't specified the curriculum type in the <code>_config.yml</code> file (current value in <code>_config.yml</code>: "<strong>{{ site.curriculum }}</strong>", possible values: <code>dc-image</code>, <code>dc-astronomy</code>, <code>dc-ecology</code>, <code>dc-genomics</code>, <code>dc-socsci</code>, or <code>dc-geospatial</code>). After editing this file, you need to run <code>make serve</code> again to see the changes reflected.
</div>
{% endunless %}
{% endif %}

{% comment %}
Check SWC curriculum
{% endcomment %}

{% if site.carpentry == "swc" %}
{% unless site.curriculum == "swc-inflammation" or site.curriculum == "swc-gapminder" %}
<div class="alert alert-warning">
It looks like you are setting up a website for a Software Carpentry curriculum but you haven't specified the curriculum type in the <code>_config.yml</code> file (current value in <code>_config.yml</code>: "<strong>{{ site.curriculum }}</strong>", possible values: <code>swc-inflammation</code>, or <code>swc-gapminder</code>). After editing this file, you need to run <code>make serve</code> again to see the changes reflected.
</div>
{% endunless %}
{% endif %}

{% comment %}
EVENTBRITE

This block includes the Eventbrite registration widget if
'eventbrite' has been set in the header.  You can delete it if you
are not using Eventbrite, or leave it in, since it will not be
displayed if the 'eventbrite' field in the header is not set.
{% endcomment %}
{% if page.eventbrite %}
<strong>Some adblockers block the registration window. If you do not see the
  registration box below, please check your adblocker settings.</strong>
<iframe
  src="https://www.eventbrite.com/tickets-external?eid={{page.eventbrite}}&ref=etckt"
  frameborder="0"
  width="100%"
  height="280px"
  scrolling="auto">
</iframe>
{% endif %}


<h2 id="general">Información General</h2>

{% comment %}
INTRODUCTION

Edit the general explanatory paragraph below if you want to change
the pitch.
{% endcomment %}

<p>
El proyecto <strong><a href="https://carpentries.org">The Carpentries</a></strong> incluye las comunidades de instructores, formadores, mantenedores, ayudantes y personal de apoyo de <a
href="{{site.swc_site}}">Software Carpentry</a>, <a href="{{site.dc_site}}">Data Carpentry</a>, y
<a href="{{site.lc_site}}">Library Carpentry</a> que comparten la misión de enseñar habilidades básicas de computación y ciencia de datos a los investigadores.

<p align="center">
  <em>

  <strong>¿Quiere obtener más información y seguir interactuando con The Carpentries? </strong> Carpentries Clippings es el boletín quincenal de The Carpentries, donde compartimos noticias de la comunidad, ofertas de trabajo de la comunidad y más. Regístrese para recibir ediciones futuras y leer nuestro archivo completo: <a href="https://carpentries.org/newsletter/">https://carpentries.org/newsletter/</a>

  </em>
</p>
{% if site.carpentry == "swc" %}
{% include swc/intro.html %}
{% elsif site.carpentry == "dc" %}
{% include dc/intro.html %}
{% elsif site.carpentry == "lc" %}
{% include lc/intro.html %}
{% endif %}

{% if site.pilot %}
This is a pilot workshop, testing out a lesson that is still under development. The lesson authors would appreciate any feedback you can give them about the lesson content and suggestions for how it could be further improved.
{% endif %}

{% comment %}
AUDIENCE

Explain who your audience is.  (In particular, tell readers if the
workshop is only open to people from a particular institution.
{% endcomment %}

{% if site.carpentry == "swc" %}
{% include swc/who.html %}
{% elsif site.carpentry == "dc" %}
{% include dc/who.html %}
{% elsif site.carpentry == "lc" %}
{% include lc/who.html %}
{% endif %}

{% comment %}
LOCATION

This block displays the address and links to maps showing directions
if the latitude and longitude of the workshop have been set.  You
can use https://www.latlong.net/ to find the lat/long of an
address.
{% endcomment %}

{% assign begin_address = page.address | slice: 0, 4 | downcase  %}
{% if page.address == "online" %}
{% assign online = "true_private" %}
{% elsif begin_address contains "http" %}
{% assign online = "true_public" %}
{% else %}
{% assign online = "false" %}
{% endif %}
{% if page.latitude and page.longitude and online == "false" %}
<p id="where">
  <strong>Dónde:</strong>
  {{page.address}}.
  Para detalles de dirección y cómo llegar checa <strong><a href="https://csvconf.com/location/location-es/">Cómo llegar</a></strong> en la página web del congreso.
  
  Ver direcciones con
  <a href="//www.openstreetmap.org/?mlat={{page.latitude}}&mlon={{page.longitude}}&zoom=16">OpenStreetMap</a>
  o
  <a href="//maps.google.com/maps?q={{page.latitude}},{{page.longitude}}">Google Maps</a>.

</p>
{% elsif online == "true_public" %}
<p id="where">
  <strong>Dónde:</strong>
  online at <a href="{{page.address}}">{{page.address}}</a>.
  If you need a password or other information to access the training,
  the instructor will pass it on to you before the workshop.
</p>
{% elsif online == "true_private" %}
<p id="where">
  <strong>Dónde:</strong> This training will take place online.
  The instructors will provide you with the information you will need to connect to this meeting.
</p>
{% endif %}

{% comment %}
DATE

This block displays the date and links to Google Calendar.
{% endcomment %}
{% if page.humandate %}
<p id="when">
  <strong>Cuando:</strong>
  {{page.humandate}}.
  {% include workshop_calendar.html %}
</p>
{% endif %}

{% comment %}
SPECIAL REQUIREMENTS

Modify the block below if there are any special requirements.
{% endcomment %}
<p id="requirements">
  <strong>Requisitos previos:</strong>
  {% if online == "false" %}
    Los participantes deben tener acceso a una computadora con
    Sistema operativo Mac, Linux o Windows (no una tableta, Chromebook, etc.) con privilegios de administración.
  {% else %}
    Los participantes deben tener acceso a una computadora con
    Sistema operativo Mac, Linux o Windows (no una tableta, Chromebook, etc.) con privilegios de administración.
  {% endif %}
  Deben tener algunos paquetes de software específicos instalados (listados <a href="#setup">abajo</a>).
</p>

{% comment %}
ACCESSIBILITY

Modify the block below if there are any barriers to accessibility or
special instructions.
{% endcomment %}
<p id="accessibility">
  <strong>Accesibilidad:</strong>
{% if online == "false" %}
  Estamos comprometidos a hacer de este taller
  accesible a todos. Para los talleres en un lugar físico, los organizadores del taller han comprobado que:
</p>
<ul>
  <li>El salón es accesible para sillas de ruedas o scooters.</li>
  <li>Hay baños accesibles disponibles.</li>
</ul>
<p>
  Los materiales se proporcionarán antes del taller y
  folletos en letra grande están disponibles previa notificación a los
  organizadores. Si podemos ayudar a que el aprendizaje sea más fácil para
  usted (por ejemplo, intérpretes de lengua de señas, instalaciones de lactancia), por favor
  póngase en contacto (utilizando los datos de contacto a continuación) e
  intentarémos proporcionárselos.
</p>
{% else %}
  We are dedicated to providing a positive and accessible learning environment for all. 
  We do not require participants to provide documentation of disabilities or disclose any unnecessary personal information. 
  However, we do want to help create an inclusive, accessible experience for all participants. 
  We encourage you to share any information that would be helpful to make your Carpentries experience accessible.
  To request an accommodation for this workshop, please fill out the 
  <a href="https://carpentries.typeform.com/to/B2OSYaD0">accommodation request form</a>.
  If you have questions or need assistance with the accommodation form please <a href="mailto:team@carpentries.org">email us</a>.
</p>
{% endif %}

{% comment %}
CONTACT EMAIL ADDRESS

Display the contact email address set in the configuration file.
{% endcomment %}
<p id="contact">
  <strong>Contacto:</strong>
  Por favor envíe un correo electrónico 
  {% if page.email %}
  {% for email in page.email %}
  {% if forloop.last and page.email.size > 1 %}
  o
  {% else %}
  {% unless forloop.first %}
  ,
  {% endunless %}
  {% endif %}
  <a href='mailto:{{email}}'>{{email}}</a>
  {% endfor %}
  {% else %}
  to-be-announced
  {% endif %}
  para más información.
</p>

<p id="roles">
  <strong>Roles:</strong>
  Para obtener más información sobre los roles en el taller (quién hará qué), consulte nuestras <a href="https://carpentries.org/workshop_faq/#what-are-the-roles-of-everyone-participating-in-a-workshop">Preguntas frecuentes</a> sobre el taller.
</p>

{% comment %}
<p> tag to make this section visible.

Edit the text to match who can attend the workshop. For instance:
- This workshop is open to affiliates to ABC university.
- This workshop is open to the public.
- If you are interested in attending this workshop, contact me@example.com
  for more information
{% endcomment %}

<p id="who-can-attend">
    <strong>Quién puede asistir?:</strong>
    El taller esta enfocado a principiantes interesados en aprender a programar en python.
</p>


<hr/>

{% comment%}
REGISTRO
{% endcomment %}
<h2 id="register">Registro</h2>
Es necesario <strong>REGISTRARSE</strong> llenando la 
<a href="https://forms.gle/zh3d5aH8qpxgeQis9">
    <button type="button" class="btn btn-info">Solicitud de Inscripción. </button>
  </a>
( Preferentemente usa el navegador Chrome para abrir la página ).

<br>
<br>
La solicitud será evaluada por el comité y le dará una respuesta a través del correo electrónico que proporcionó en la solicitud. Si por causas de fuerza mayor no puede asistir al taller, favor de responder en el mismo correo, para dar espacio a otras personas interesadas.


<br>
<br>
<strong>El cupo esta limitado a 30 participantes.</strong>

<!-- FONT COLOR="red"><strong>CUPO LLENO.</strong></FONT> Agradecemos tu participación -->
<p>

</p>

<hr/>

{% comment%}
CODE OF CONDUCT
{% endcomment %}
<h2 id="code-of-conduct">Código de Conducta</h2>

<p>
Todas las personas que participan en las actividades de Carpentries deben cumplir con el <a href="https://docs.carpentries.org/topic_folders/policies/code-of-conduct.html">Código de Conducta</a>. Este documento también describe cómo informar un incidente si es necesario.
</p>

<p class="text-center">
  <a href="https://goo.gl/forms/KoUfO53Za3apOuOK2">
    <button type="button" class="btn btn-info">Reporta un incidente del código de conducta</button>
  </a>
</p>
<hr/>


{% comment %}
Collaborative Notes

If you want to use an Etherpad, go to

https://pad.carpentries.org/YYYY-MM-DD-site

where 'YYYY-MM-DD-site' is the identifier for your workshop,
e.g., '2015-06-10-esu'.

Note we also have a CodiMD (the open-source version of HackMD)
available at https://codimd.carpentries.org
{% endcomment %}
{% if page.collaborative_notes %}
<h2 id="collaborative_notes">Notas Colaborativas</h2>

<p>
Usaremos este  <a href="{{ page.collaborative_notes }}">documento colaborativo</a> para chatear, tomar notas y compartir URL y fragmentos de código.
</p>
<hr/>
{% endif %}


{% comment %}
SURVEYS - DO NOT EDIT SURVEY LINKS
{% endcomment %}
<h2 id="surveys">Encuestas</h2>
<p>Asegúrese de completar estas encuestas antes y después del taller.</p>
{% if site.carpentry == "incubator" %}
<p><a href="{{ site.incubator_pre_survey }}">Encuesta previa al taller</a></p>
<p><a href="{{ site.incubator_post_survey }}">Encuesta posterior al taller</a></p>
{% elsif site.incubator_pre_survey or site.incubator_post_survey %}
<div class="alert alert-danger">
WARNING: you have defined custom pre- and/or post-survey links for
a workshop not configured for The Carpentries Incubator
(the value of `curriculum` is not set to `incubator` in `_config.yml`).
Please comment out the `incubator_pre_survey` and `incubator_post_survey` fields
in `_config.yml` or, if this workshop is teaching a lesson in the Incubator,
change the value of `carpentry` to `incubator`.
</div>
{% else %}
<p><a href="{{ site.pre_survey }}{{ site.github.project_title }}">Encuesta previa al taller</a></p>
<p><a href="{{ site.post_survey }}{{ site.github.project_title }}">Encuesta posterior al taller</a></p>
{% endif %}

<hr/>


{% comment %}
SCHEDULE

Show the workshop's schedule.

Small changes to the schedule can be made by modifying the
`schedule.html` found in the `_includes` folder for your
workshop type (`swc`, `lc`, or `dc`). Edit the items and
times in the table to match your plans. You may also want to
change 'Day 1' and 'Day 2' to be actual dates or days of the
week.

For larger changes, a blank template for a 4-day workshop
(useful for online teaching for instance) can be found in
`_includes/custom-schedule.html`. Add the times, and what
you will be teaching to this file. You may also want to add
rows to the table if you wish to break down the schedule
further. To use this custom schedule here, replace the block
of code below the Schedule `<h2>` header below with
`{% include custom-schedule.html %}`.
{% endcomment %}

<h2 id="schedule">Calendario de Actividades</h2>

{% if site.carpentry == "swc" %}
{% include swc/schedule.html %}
{% elsif site.carpentry == "dc" %}
{% include dc/schedule.html %}
{% elsif site.carpentry == "lc" %}
{% include lc/schedule.html %}
{% elsif site.carpentry == "incubator" %}
This workshop is teaching a lesson in [The Carpentries Incubator](https://carpentries-incubator.org/).
Please check [the lesson homepage]({{ site.incubator_lesson_site }}) for a list of lesson sections and estimated timings.
{% endif %}

{% comment %}
Edit/replace the text above if you want to iSchedulenclude a schedule table.
See the contents of the _includes/custom-schedule.html file for an example of
how one of these schedule tables is constructed.
{% endcomment %}

{% if site.pilot %}
The lesson taught in this workshop is being piloted and a precise schedule is yet to be established. The workshop will include regular breaks. Please [contact the workshop organisers](#contact) if you would like more information about the planned schedule.
{% endif %}

<hr/>


{% comment %}
SETUP

Delete irrelevant sections from the setup instructions.  Each
section is inside a 'div' without any classes to make the beginning
and end easier to find.

This is the other place where people frequently make mistakes, so
please preview your site before committing, and make sure to run
'tools/check' as well.
{% endcomment %}

<h2 id="setup">Configuración</h2>

<p>
  Para participar en un taller de
  {% if site.carpentry == "swc" %}
  Software Carpentry
  {% elsif site.carpentry == "dc" %}
  Data Carpentry
  {% elsif site.carpentry == "lc" %}
  Library Carpentry
  {% endif %}
  ,
  necesitará acceso al software como se describe a continuación.
  Además, necesitará un navegador web actualizado.
</p>
<p>
  Mantenemos una lista de problemas comunes que ocurren durante la instalación como referencia para los instructores que pueden ser útiles en la página wiki de <a href = "{{site.swc_github}}/workshop-template/wiki/Configuration-Problems-and-Solutions">Problemas y soluciones de configuración</a>.
</p>

{% comment %}
For online workshops, the section below provides:
- installation instructions for the Zoom client
- recommendations for setting up Learners' workspace so they can follow along
  the instructions and the videoconferencing

If you do not use Zoom for your online workshop, edit the file
`_includes/install_instructions/videoconferencing.html`
to include the relevant installation instructions.
{% endcomment %}
{% if online != "false" %}
{% include install_instructions/videoconferencing.html %}
{% endif %}

{% comment %}
These are the installation instructions for the tools used
during the workshop.
{% endcomment %}

{% if site.carpentry == "swc" %}
{% include swc/setup.html %}
{% elsif site.carpentry == "dc" %}
{% include dc/setup.html %}
{% elsif site.carpentry == "lc" %}
{% include lc/setup.html %}
{% elsif site.carpentry == "incubator" %}
Please check the "Setup" page of
[the lesson site]({{ site.incubator_lesson_site }}) for instructions to follow
to obtain the software and data you will need to follow the lesson.
{% endif %}

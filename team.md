---
layout: default
permalink: /team/
---

<div class="container-fluid" >
    <center>
        <div style="padding-bottom:50px;"><h2>Responsables</h2></div>
    </center>
    <div class="row-fluid">
        {% for member in site.data.team.managers %}
        <div class="col-md-6">
        <div class="table-responsive">
            <table class="table table-bordered table-hover table-striped" style="margin-top:50px">
                <tbody>
                <tr>
                 <td colspan="2" style="text-align:center"><h3>{{ member.position }}</h3></td>
                </tr>
                <tr>
                <td>
                {% if member.photo %}
                    <img src="{{ member.photo }}" width="128px">
                {% else %}
                 <img src="/images/photos/unknown-id-128x128.png" width="128px">
                {% endif %}
                </td>
                    <td>
                        <ul>
                            <li>{{ member.name }}</li>
                            <li>Bureau: {{ member.office }}</li>
                            <li>E-mail: <a href="mailto:{{ member.email }}">{{ member.email }}</a></li>
                            <li>Téléphone: {{ member.telephone }}</li>
                        </ul>
                    </td>
                </tr>
                </tbody>
            </table>

        </div>
            </div>
        {% endfor %}
</div>
</div>

<div class="container-fluid">
    <center>
        <div style="padding-bottom:50px;"><h2>&Eacute;quipe pédagogique</h2></div>
    </center>
    <div class="row-fluid">

        {% for member in site.data.team.members %}
        <div class="col-md-6">
        <a class="anchor" id="{{ member.id }}"></a>
        <div class="table-reponsive">
            <table class="table table-bordered table-hover table-striped" style="margin-top:50px">
                <tbody>
                <tr>
                    <td colspan="2" style="text-align:center"><h3>{{ member.name }}</h3></td>
                </tr>
                <tr>
                <td>
                {% if member.photo %}
                    <img src="{{ member.photo }}" width="128px">
                {% else %}
                 <img src="/images/photos/unknown-id-128x128.png" width="128px">
                {% endif %}
                </td>
                    <td>
                        <ul>
                            {% if member.office %}
                                <li>Bureau: {{ member.office }}</li>
                            {% endif %}
                            <li>E-mail: <a href="mailto:{{ member.email }}">{{ member.email }}</a></li>
                            {% if member.telephone %}
                                <li>Téléphone: {{ member.telephone }}</li>
                            {% endif %}
                            <li>Cours:
                             <ul>
                            {% assign course = | member.course | split:";" %}
                            {% for id in course %}
                             {% for course in site.data.course.courseS1 %}
         {% if course.id == id %}
          {% assign name = course.name %}
         {% endif %}
        {% endfor %}

        {% for course in site.data.course.courseS2 %}
         {% if course.id == id %}
          {% assign name = course.name %}
         {% endif %}
        {% endfor %}

        {% for course in site.data.course.courseS2UEChoice %}
         {% if course.id == id %}
          {% assign name = course.name %}
         {% endif %}
        {% endfor %}

        {% for course in site.data.course.courseS3 %}
         {% if course.id == id %}
          {% assign name = course.name %}
         {% endif %}
        {% endfor %}

                                {% for course in site.data.course.courseS4 %}
         {% if course.id == id %}
          {% assign name = course.name %}
         {% endif %}
        {% endfor %}

                                <li><a href="/course/#{{ id }}">{{ name }}</a></li>

                            {% endfor %}
                             </ul>
                            </li>
                        </ul>
                    </td>
                </tr>
                </tbody>
            </table>
        </div>
        </div>
        {% endfor %}
    </div>
</div>

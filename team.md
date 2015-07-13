---
layout: default
permalink: /team/
---

<div class="container-fluid" >
    <center>
        <div style="padding-bottom:50px;"><h2>Responsables</h2></div>
    </center>
    <div class="row-fluid">
    <div class="col-md-3"></div>
        <div class="col-md-6">

        {% for member in site.data.team.managers %}

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
        {% endfor %}

          </div>
          <div class="col-md-3"></div>
    </div>
</div>

<div class="container" style="max-width:600px">
    <center>
        <div style="padding-bottom:50px;"><h2>&Eacute;quipe pédagogique</h2></div>
    </center>
    <div class="row-fluid">

        {% for member in site.data.team.members %}
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
                                	<li><a href="/course/#{{ id }}">{{ id }}</a></li>
                            {% endfor %}
                            	</ul>
                            </li>
                        </ul>
                    </td>
                </tr>
                </tbody>
            </table>
        </div>
        {% endfor %}
    </div>
</div>
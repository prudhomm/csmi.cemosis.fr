---
layout: default
permalink : /course/
---

<div class="container-fluid">
	<div class="row-fluid">
		<div class="col-md-3">
		<div id="toc"></div>
		</div>

		<div class="col-md-6" >
		<a class="anchor" id="S1"></a>
		<div style="text-align:center"><h1>Semestre 1</h1></div>

		{% for course in site.data.course.courseS1 %}
			<a class="anchor" id="{{ course.id }}">{{ course.name }}</a>
			<table class="table table-bordered table-striped" style="margin-top:50px">
				<tbody>
				<tr style="background-color:#CCCCCC">
					<td style="text-align:center"><h2>{{ course.name }}</h2></td>
				</tr>
				<tr>
					<td>
						<h3>Contenu</h3>
						<p>{{ course.content }}</p>
						<h3>Objectifs : savoir-faire et compétences</h3>
						<p>{{ course.knowledege }}</p>
						<h3>Autres informations</h3>
						<p>{{ course.info }}</p>
						<h3>Enseignant(s):</h3>
							{% if course.teacher %}
							<ul>
								{% assign teacher = | course.teacher | split:";" %}
								{% for id in teacher %}
									{% for member in site.data.team.members %}
											{% if member.id == id %}
											{% assign name = member.name %}
											{% endif %}
									{% endfor %}		
								<li><a href="/team/#{{ id }}">{{ name }}</a></li>

								{% endfor %}
							</ul>
							{% else %}
							<br>
							{% endif %}

						<table class="table table-bordered table-striped">
							<tr>
								<td style="text-align:center"><h3>Volume horaire</h3></td>
							</tr>
							<tr>
								<td><p>{{ course.duration }}</p></td>
							</tr>
						</table>
					</td>
				</tr>
				</tbody>
			</table>

		{% endfor %}
			<a class="anchor" id="S2"></a>
			<div style="text-align:center"><h1>Semestre 2</h1></div>

		{% for course in site.data.course.courseS2 %}


			<a class="anchor" id="{{ course.id }}">{{ course.name }}</a>
			<table class="table table-bordered table-striped" style="margin-top:50px">
				<tbody>
				<tr style="background-color:#CCCCCC">
					<td style="text-align:center"><h2>{{ course.name }}</h2></td>
				</tr>
				<tr>
					<td>
						<h3>Contenu</h3>
						<p>{{ course.content }}</p>
						<h3>Objectifs : savoir-faire et compétences</h3>
						<p>{{ course.knowledege }}</p>
						<h3>Autres informations</h3>
						<p>{{ course.info }}</p>
						<h3>Enseignant(s):</h3>
							{% if course.teacher %}
							<ul>
								{% assign teacher = | course.teacher | split:";" %}
								{% for id in teacher %}
									{% for member in site.data.team.members %}
										{% if member.id == id %}
										{% assign name = member.name %}
										{% endif %}
									{% endfor %}	
								<li><a href="/team/#{{ id }}">{{ name }}</a></li>
								{% endfor %}
							</ul>
							{% else %}
							<br>
							{% endif %}

						<table class="table table-bordered table-striped">
							<tr>
								<td><h3>Volume horaire</h3></td>
							</tr>
							<tr>
								<td style="text-align:center"><p>{{ course.duration }}</p></td>
							</tr>
						</table>
					</td>
				</tr>
				</tbody>
			</table>

		{% endfor %}

		{% for course in site.data.course.courseS2UEChoice %}

			<a class="anchor" id="{{ course.id }}">{{ course.name }}</a>
			<table class="table table-bordered table-striped" style="margin-top:50px">
				<tbody>
				<tr style="background-color:#CCCCCC">
					<td style="text-align:center"><h2>{{ course.name }}</h2></td>
				</tr>
				<tr>
					<td>
						<h3>Contenu</h3>
						<p>{{ course.content }}</p>
						<h3>Objectifs : savoir-faire et compétences</h3>
						<p>{{ course.knowledege }}</p>
						<h3>Autres informations</h3>
						<p>{{ course.info }}</p>
						<h3>Enseignant(s):</h3>
							{% if course.teacher %}
							<ul>
								{% assign teacher = | course.teacher | split:";" %}
								{% for id in teacher %}
								{% for member in site.data.team.members %}
										{% if member.id == id %}
										{% assign name = member.name %}
										{% endif %}
									{% endfor %}	
								<li><a href="/team/#{{ id }}">{{ name }}</a></li>
								{% endfor %}
							</ul>
							{% else %}
							<br>
							{% endif %}

						<table class="table table-bordered table-striped">
							<tr>
								<td><h3>Volume horaire</h3></td>
							</tr>
							<tr>
								<td style="text-align:center"><p>{{ course.duration }}</p></td>
							</tr>
						</table>
					</td>
				</tr>
				</tbody>
			</table>

		{% endfor %}
			<a class="anchor" id="S3"></a>
			<div style="text-align:center"><h1>Semestre 3</h1></div>

		{% for course in site.data.course.courseS3 %}

			<a class="anchor" id="{{ course.id }}">{{ course.name }}</a>
			<table class="table table-bordered table-striped" style="margin-top:50px">
				<tbody>
				<tr style="background-color:#CCCCCC">
					<td style="text-align:center"><h2>{{ course.name }}</h2></td>
				</tr>
				<tr>
					<td>
						<h3>Contenu</h3>
						<p>{{ course.content }}</p>
						<h3>Objectifs : savoir-faire et compétences</h3>
						<p>{{ course.knowledege }}</p>
						<h3>Autres informations</h3>
						<p>{{ course.info }}</p>
						<h3>Enseignant(s):</h3>
							{% if course.teacher %}
							<ul>
								{% assign teacher = | course.teacher | split:";" %}
								{% for id in teacher %}
								{% for member in site.data.team.members %}
										{% if member.id == id %}
										{% assign name = member.name %}
										{% endif %}
									{% endfor %}	
								<li><a href="/team/#{{ id }}">{{ name }}</a></li>
								{% endfor %}
							</ul>
							{% else %}
							<br>
							{% endif %}
						<table class="table table-bordered table-striped">
							<tr>
								<td><h3>Volume horaire</h3></td>
							</tr>
							<tr>
								<td style="text-align:center"><p>{{ course.duration }}</p></td>
							</tr>
						</table>
					</td>
				</tr>
				</tbody>
			</table>

		{% endfor %}
			<a class="anchor" id="S4"></a>
			<div style="text-align:center"><h1>Semestre 4</h1></div>

		{% for course in site.data.course.courseS4 %}

			<a class="anchor" id="{{ course.id }}">{{ course.name }}</a>
			<table class="table table-bordered table-striped" style="margin-top:50px">
				<tbody>
				<tr style="background-color:#CCCCCC">
					<td style="text-align:center"><h2>{{ course.name }}</h2></td>
				</tr>
				<tr>
					<td>
						<h3>Contenu</h3>
						<p>{{ course.content }}</p>
						<h3>Objectifs : savoir-faire et compétences</h3>
						<p>{{ course.knowledege }}</p>
						<h3>Autres informations</h3>
						<p>{{ course.info }}</p>
						<h3>Enseignant(s):</h3>
							{% if course.teacher %}
							<ul>
								{% assign teacher = | course.teacher | split:";" %}
								{% for id in teacher %}
									{% for member in site.data.team.members %}
										{% if member.id == id %}
										{% assign name = member.name %}
										{% endif %}
									{% endfor %}	

								<li><a href="/team/#{{ id }}">{{ name }}</a></li>
								{% endfor %}
							</ul>
							{% else %}
							<br>
							{% endif %}

						<table class="table table-bordered table-striped">
							<tr>
								<td><h3>Volume horaire</h3></td>
							</tr>
							<tr>
								<td style="text-align:center"><p>{{ course.duration }}</p></td>
							</tr>
						</table>
					</td>
				</tr>
				</tbody>
			</table>

		{% endfor %}
		</div>
		<div class="col-md-3"></div>	
	</div>
</div>
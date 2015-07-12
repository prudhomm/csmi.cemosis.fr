---
layout: default
permalink : /course/
---

<div class="container-fluid">
	<div class="row-fluid">
		<div class="col-md-3">
		<div id="toc"></div>
		</div>

		<div class="col-md-5" >

			<div style="text-align:center"><h1>Semestre 1</h1></div>

		{% for course in site.data.course.courseS1 %}
			<span class="anchor" id="{{ course.id }}">{{ course.name }}</span>
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

			<div style="text-align:center"><h1>Semestre 2</h1></div>
			
		{% for course in site.data.course.courseS2 %}


			<span class="anchor" id="{{ course.id }}">{{ course.name }}</span>
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

			<span class="anchor" id="{{ course.id }}">{{ course.name }}</span>
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

			<div style="text-align:center"><h1>Semestre 3</h1></div>

		{% for course in site.data.course.courseS3 %}

			<span class="anchor" id="{{ course.id }}">{{ course.name }}</span>
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

			<div style="text-align:center"><h1>Semestre 4</h1></div>

		{% for course in site.data.course.courseS4 %}

			<span class="anchor" id="{{ course.id }}">{{ course.name }}</span>
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
		<div class="col-md-4"></div>	
	</div>
</div>
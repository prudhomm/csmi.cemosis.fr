---
layout: default
permalink : /course/
---

<div class="container" style="max-width:800px">

{% for course in site.data.course.courseS1 %}
	<span class="anchor" id="{{ course.id }}"></span>
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

{% for course in site.data.course.courseS2 %}
	<span class="anchor" id="{{ course.id }}"></span>
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
	<span class="anchor" id="{{ course.id }}"></span>
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

{% for course in site.data.course.courseS3 %}
	<span class="anchor" id="{{ course.id }}"></span>
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

{% for course in site.data.course.courseS4 %}
	<span class="anchor" id="{{ course.id }}"></span>
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



<script>
$(document).ready(function() {
  //Calls the tocify method on your HTML div.
  $("#toc").tocify({ showEffect: "fadeIn" });
});
</script>
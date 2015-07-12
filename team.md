---
layout: default
permalink: /team/
---

<center style="margin-top:80px"><h2>&Eacute;quipe pédagogique</h2></center>

<div class="container" style="max-width:500px">

{% for member in site.data.team.members %}

	<table class="table table-bordered table-hover table-striped" style="margin-top:50px">
		<tbody>
		<tr>
			<td style="text-align:center">{{ member.name }}</td>
		</tr>
		<tr>
			<td>
				<ul>

					<li>{{ member.position }}</li>
					<li>Bureau: {{ member.office }}</li>
					<li>E-mail: <a href="mailto:{{ member.email }}">{{ member.email }}</a></li>
					<li>Téléphone: {{ member.telephone }}</li>
				</ul>
			</td>
		</tr>
		</tbody>
	</table>

{% endfor %}

</div>
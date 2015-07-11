---
layout: default
permalink: /team/
---

<center style="margin-top:80px"><h2>&Eacute;quipe pédagogique</h2></center>

<div class="container" style="margin:0 auto width:400px">

{% for member in site.data.team.members %}

	<table class="">
		<tr>
			<td>{{ member.name }}</td>
			<td>
				<ul>

					<li>{{ member.position }}</li>
					<li>{{ member.office }}</li>
					<li><a href="mailto:{{ member.email }}">{{ member.email }}</a></li>
					<li>{{ member.telephone }}</li>
				</ul>
			</td>
		</tr>
	</table>

{% endfor %}

</div>
---
layout: default
permalink: /team/
---

<center><h2>&Eacute;quipe pédagogique</h2></center>

{% for member in site.data.team.members %}

<div class="container-fluid">
	
	
	<table>
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
</div>

{% endfor %}
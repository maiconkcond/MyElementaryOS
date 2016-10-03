# MyElementaryOS
Instalação organizada dos programas e comandos pós instalação do ElementaryOS


<h2>Comandos uteis<h2>

<ul>
	<li>Listar PPAs instalados</li>
	<p>grep -RoPish "ppa.launchpad.net/[^/]+/[^/ ]+" /etc/apt | sort -u | sed -r 's/\.[^/]+\//:/'</p>
</ul>
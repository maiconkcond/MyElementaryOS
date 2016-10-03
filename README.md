# MyElementaryOS
Instalação organizada dos programas e comandos pós instalação do ElementaryOS


###Comandos uteis

*Listar PPAs instalados
```
grep -RoPish "ppa.launchpad.net/[^/]+/[^/ ]+" /etc/apt | sort -u | sed -r 's/\.[^/]+\//:/'
```

###Sistema

*GDebi - Instalar PPAs e Pacotes .deb
```
p>sudo apt install software-properties-common gdebi -y
```	

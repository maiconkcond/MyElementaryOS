# MyElementaryOS
Instalação organizada dos programas e comandos pós instalação do ElementaryOS


###Commands
* Listar PPAs instalados
```
grep -RoPish "ppa.launchpad.net/[^/]+/[^/ ]+" /etc/apt | sort -u | sed -r 's/\.[^/]+\//:/'
```

###System
* GDebi - Instalar PPAs e Pacotes .deb
```
sudo apt install software-properties-common gdebi -y
```	

* Drivers adicionais
```
sudo apt install software-properties-gtk
```

* Elementary Tweaks
```
sudo add-apt-repository -y ppa:philip.scott/elementary-tweaks && sudo apt update && sudo apt install -y elementary-tweaks

```
* Elementary Plus
```
sudo add-apt-repository ppa:cybre/elementaryplus
sudo apt-get update
sudo apt-get upgrade && sudo apt-get install elementaryplus
```

###Developer
* Git
```
sudo add-apt-repository ppa:git-core/ppa -y
sudo apt-get update
sudo apt-get install git -y
```

* Sublime3
```
sudo add-apt-repository ppa:webupd8team/sublime-text-3 -y
sudo apt-get update
sudo apt-get install sublime-text-installer -y
```

* NodeJS
```
curl -sL https://deb.nodesource.com/setup_4.x | sudo -E bash -
sudo apt-get install -y nodejs
sudo apt-get install -y build-essential
sudo apt install npm
```

* Ruby Dependencies
```
sudo apt-get install git-core curl zlib1g-dev build-essential libssl-dev libreadline-dev libyaml-dev libsqlite3-dev sqlite3 libxml2-dev libxslt1-dev libcurl4-openssl-dev python-software-properties libffi-dev
```

* Ruby
```
cd
git clone https://github.com/rbenv/rbenv.git ~/.rbenv
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc
echo 'eval "$(rbenv init -)"' >> ~/.bashrc
exec $SHELL

git clone https://github.com/rbenv/ruby-build.git ~/.rbenv/plugins/ruby-build
echo 'export PATH="$HOME/.rbenv/plugins/ruby-build/bin:$PATH"' >> ~/.bashrc
exec $SHELL

rbenv install 2.3.1
rbenv global 2.3.1
ruby -v
```

* Rails
```
gem install rails -v 4.2.6
rails -v
```

* Android Studio
```
sudo add-apt-repository ppa:ubuntu-desktop/ubuntu-make -y && sudo apt-get update && sudo apt-get install ubuntu-make -y
umake android
sudo apt-get install android-tools-adb 
```

###Softwares and Applications

* Java 8
```
sudo add-apt-repository ppa:webupd8team/java -y
sudo apt-get update
sudo apt-get install oracle-java8-installer -y
```

* Skype
```
sudo apt-add-repository "deb http://archive.canonical.com/ubuntu/ trusty partner" -y
sudo apt-get update && sudo apt-get install skype -y
sudo apt-get install gtk2-engines-murrine:i386 gtk2-engines-pixbuf:i386 -y
```

* PlayonLinux
```
wget -q "http://deb.playonlinux.com/public.gpg" -O- | sudo apt-key add -
sudo wget http://deb.playonlinux.com/playonlinux_precise.list -O /etc/apt/sources.list.d/playonlinux.list
sudo apt-get update
sudo apt-get install playonlinux -y
```

* Gedit (Text Editor)
```
sudo apt-get install gedit gedit-plugins
```

* Guake Terminal
```
sudo apt-get install guake
```

* Steam
```
wget http://repo.steampowered.com/steam/signature.gpg && sudo apt-key add signature.gpg
sudo sh -c 'echo "deb http://repo.steampowered.com/steam/ precise steam" >> /etc/apt/sources.list.d/steam.list'
sudo apt-get update
sudo apt-get install steam
```

* Libre Office 4
```
sudo add-apt-repository ppa:libreoffice/libreoffice-4-0
sudo apt-get update
sudo apt-get install libreoffice
```

* Spotify
```
sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys BBEBDCB318AD50EC6865090613B00F1FD2C19886
echo deb http://repository.spotify.com stable non-free | sudo tee /etc/apt/sources.list.d/spotify.list
sudo apt-get update
sudo apt-get install spotify-client
```

* Clementine Music Player
```
sudo add-apt-repository ppa:me-davidsansome/clementine
sudo apt-get update
sudo apt-get install clementine
```

* VirtualBox
```
wget -q http://download.virtualbox.org/virtualbox/debian/oracle_vbox.asc -O- | sudo apt-key add -
sudo sh -c 'echo "deb http://download.virtualbox.org/virtualbox/debian precise contrib" >> /etc/apt/sources.list.d/virtualbox.list'
sudo apt-get update
sudo apt-get install virtualbox-4.3
```



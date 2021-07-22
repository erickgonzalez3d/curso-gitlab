# cusrso de gitlab 

este curso esta hecho desde windows usando ubuntu con wsl y no como una maquina virtual y no se centra en el manejo de git, para eso esta el curso de git 

Debemos tener instalado git y ubuntu en windows 

git lo descargamos de la pagina oficial y ubuntu del microsoft store, trabajaremos con el 18.04 LTS  y lo dejamos en la carpeta por defecto, no cambiamos la ruta de instalación  

abrimos ubuntu y ejecutamos el sudo apt get update
despues el sudo apt get upgrade y nuevamente el sudo apt get update 

vamos a gitlab.com en la pestaña install gitlab y la opcion de ubuntu 

y ejecutamos los comandos para instalar las dependencia desde donde instalaremos gitlab 

sudo apt-get update
sudo apt-get install -y curl openssh-server ca-certificates

instalamos postfix para enviar correos de notificación y le decimos que vamos a trabajar en local 

sudo apt-get install -y postfix

agregamos el repositorio de paquete 

curl https://packages.gitlab.com/install/repositories/gitlab/gitlab-ee/script.deb.sh | sudo bash

instalamos gitlab con 

sudo apt-get install gitlab-ee

y esperamos unos minutos la instalación y le reconfiguramos con el comando 

sudo gitlab-ctl reconfigure




vamos a la pagina de gitlab creamos una cuenta 


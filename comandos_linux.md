
# comandos ms usados en linux
# Ejemplo para sed y awk
CONTAINER ID        IMAGE                            COMMAND                  CREATED             STATUS                       PORTS               NAMES
53507539184a        lordjea/priv:jenkins-accelya-2   "/sbin/tini -- /usr/…"   6 months ago        Exited (137) 6 months ago                        jenkins-accelya-new2
2a7819deb6d6        python:3                         "bash"                   9 months ago        Exited (0) 9 months ago                          stoic_ptolemy
d9afaba5955e        python:3                         "bash"                   9 months ago        Exited (0) 9 months ago                          hopeful_shockley
750d20cb7092        lordjea/priv:nginx-accelya-2     "nginx -g 'daemon of…"   12 months ago       Exited (1) 12 months ago                         nginx-accelya
0618de56a259        b137a5753eb1                     "/bin/sh -c 'apt-get…"   12 months ago       Exited (100) 12 months ago                       determined_morse
f8eacdfab3c8        lordjea/jenkins-accelya:1        "/sbin/tini -- /usr/…"   12 months ago       Exited (143) 12 months ago                       jenkins-accelya

# sed
docker ps -a | sed 's/python/vibora/'
jzambrano@bildermaus:~/accelya$ docker ps -a | sed 's/python/vibora/'
CONTAINER ID        IMAGE                            COMMAND                  CREATED             STATUS                       PORTS               NAMES
53507539184a        lordjea/priv:jenkins-accelya-2   "/sbin/tini -- /usr/…"   6 months ago        Exited (137) 6 months ago                        jenkins-accelya-new2
2a7819deb6d6        vibora:3                         "bash"                   9 months ago        Exited (0) 9 months ago                          stoic_ptolemy
d9afaba5955e        vibora:3                         "bash"                   9 months ago        Exited (0) 9 months ago                          hopeful_shockley
750d20cb7092        lordjea/priv:nginx-accelya-2     "nginx -g 'daemon of…"   12 months ago       Exited (1) 12 months ago                         nginx-accelya
0618de56a259        b137a5753eb1                     "/bin/sh -c 'apt-get…"   12 months ago       Exited (100) 12 months ago                       determined_morse
f8eacdfab3c8        lordjea/jenkins-accelya:1        "/sbin/tini -- /usr/…"   12 months ago       Exited (143) 12 months ago                       jenkins-accelya

# awk
docker ps -a | sed 's/python/vibora/'
jzambrano@bildermaus:~/accelya$ docker ps -a | awk '{print $1}'
CONTAINER
53507539184a
2a7819deb6d6
d9afaba5955e
750d20cb7092
0618de56a259
f8eacdfab3c8

date
shutdown -h now 
poweroff 
mount
df
echo
less
cat
grep
watch
ping
curl
cat /etc/*release (muestra la version de la distro)
set +x
export
alias
wc
tail
head
mv
cp
rm
ping
curl
xargs
top
ps
ip a s (ver la ip de la maquina)

#ssh
ssh
scp

# para Programar scripts
source ../conf/scripts.cfg
asignacion de variables:
REMOTeHOME="/home/automata1"
if
time
export

# Tuberias |
# Redirecciones <> 



# Git
git clone # copia el repositorio remoto en la maquina donde este
git commit # guarda los cambiar en el repositorio local
git push # sube los cambios guardados al repositorio remoto
git pull # descargar los cambios nuevos que se hayan producido en el repositorio remoto


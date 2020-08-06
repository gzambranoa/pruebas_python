# Ejecutar como root
# actualizar repositorios e instalar el servidor SSH
apt update && apt install -y openssh-server \
  sudo \
  git

# crear un usuario
adduser gzambrano
#useradd -s /bin/bash -m gzambrano

# asignando permisos de sudo al usuario gzambrano
echo "gzambrano ALL=(ALL:ALL) NOPASSWD:ALL" > /etc/sudoers.d/gzambrano

# Clone del repo de scripts
git clone https://github.com/gzambranoa/pruebas_python.git


# Guardar cambios en el repo local
#git commit

# Subir cambios al repo remoto
#git push

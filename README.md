# toolbox

1. [Настройка Debian](#Настройка-Debian)

# Настройка Debian
## Заходим по su:
/usr/sbin/usermod -aG sudo subbotin
## Далее добавляем, чтобы не вводить пароль на sudo
echo "$USER ALL=(ALL:ALL) NOPASSWD: ALL" | sudo tee /etc/sudoers.d/$USER
## Ставим программы
sudo aptitude update && sudo aptitude -y upgrade
sudo aptitude install -y vim terminator

## ДЗ Подготовка базового образа VM при помощи Packer
Полезные ссылки для потомков:
```
https://ru.hexlet.io/courses/intro_to_git/lessons/gitignore/theory_unit
```
## ДЗ Основные сервисы Yandex Cloud
```
testapp_IP = 51.250.77.25
testapp_port = 9292
```
Полезные ссылки для потомков:
```
https://blog.tataranovich.com/2018/08/git-chmod.html
```
## ДЗ Знакомство с облачной инфраструктурой и облачными сервисами
```
bastion_IP = 158.160.98.219
someinternalhost_IP = 10.128.0.25
```
dns - https://www.testmyhomework.ru/

ssl сертификат установлен

Подключение к someinternalhost одной коммандой
```
ssh -i appuser@158.160.98.219 appuser@10.128.0.25
```
Для подключения через алиас необходим конфиг
```
Host bastion
  HostName 158.160.98.219
  User appuser

Host someinternalhost
  HostName 10.128.0.25
  User appuser
  ProxyJump bastion
```
Полезные ссылки для потомков:
```
https://habr.com/ru/companies/cloud4y/articles/530516/
https://wiki.gentoo.org/wiki/SSH_jump_host
https://itsecforu.ru/2019/05/06/%F0%9F%90%A7-%D0%BA%D0%B0%D0%BA-%D1%81%D0%BE%D0%B7%D0%B4%D0%B0%D1%82%D1%8C-%D0%B0%D0%BB%D0%B8%D0%B0%D1%81-ssh-%D0%B2-linux/
https://serverfault.com/questions/843243/ssh-jumping-with-aliases-and-f
https://www.digitalocean.com/community/tutorials/how-to-set-up-and-configure-an-openvpn-server-on-ubuntu-20-04#step-12-generating-client-configurations
https://docs.pritunl.com/docs/connecting
```

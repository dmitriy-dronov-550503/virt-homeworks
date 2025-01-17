
# Домашнее задание к занятию "2. Применение принципов IaaC в работе с виртуальными машинами"

## Как сдавать задания

Обязательными к выполнению являются задачи без указания звездочки. Их выполнение необходимо для получения зачета и диплома о профессиональной переподготовке.

Задачи со звездочкой (*) являются дополнительными задачами и/или задачами повышенной сложности. Они не являются обязательными к выполнению, но помогут вам глубже понять тему.

Домашнее задание выполните в файле readme.md в github репозитории. В личном кабинете отправьте на проверку ссылку на .md-файл в вашем репозитории.

Любые вопросы по решению задач задавайте в чате учебной группы.

---


## Важно!

Перед отправкой работы на проверку удаляйте неиспользуемые ресурсы.
Это важно для того, чтоб предупредить неконтролируемый расход средств, полученных в результате использования промокода.

Подробные рекомендации [здесь](https://github.com/netology-code/virt-homeworks/blob/virt-11/r/README.md)

---

## Задача 1

- Опишите своими словами основные преимущества применения на практике IaaC паттернов.
- Какой из принципов IaaC является основополагающим?

---
**Решение**

Основными преимуществами применения IaaC паттернов является простота и эффективность конфигурирования,
описание инфраструктуры как кода, что позволяет одновременно её документировать и является основополагающим
приницпом IaaC. Таким образом появляется возможность унифицированной настройки всего окружения, 
перенос этих настроек в другое место при необходимости, а также простота управления инфраструктурой 
и изменения конфигурации.

---

## Задача 2

- Чем Ansible выгодно отличается от других систем управление конфигурациями?
- Какой, на ваш взгляд, метод работы систем конфигурации более надёжный push или pull?

---
**Решение**

Ansible использует язык python, и производит конфигурацию через SSH, что делает его наиболее удобным
для применения, поскольку не требует установки дополнительных программ.


Наиболее надёжным методом работы систем конфигурации является push, потому что позволяет управлять множеством узлов
из одной главной точки, быть ведущим, в то время как pull подчиняется множеству узлов и делает управляющий узел ведомым.

---

## Задача 3

Установить на личный компьютер:

- VirtualBox
- Vagrant
- Ansible

*Приложить вывод команд установленных версий каждой из программ, оформленный в markdown.*

---
**Решение**

```
dmdmdr@ubuntu-station:~$ vboxmanage --version
6.1.38_Ubuntur153438
dmdmdr@ubuntu-station:~$ vagrant --version
Vagrant 2.2.6
dmdmdr@ubuntu-station:~$ ansible --version
ansible 2.9.6
  config file = /etc/ansible/ansible.cfg
  configured module search path = ['/home/dmdmdr/.ansible/plugins/modules', '/usr/share/ansible/plugins/modules']
  ansible python module location = /usr/lib/python3/dist-packages/ansible
  executable location = /usr/bin/ansible
  python version = 3.8.10 (default, Jun 22 2022, 20:18:18) [GCC 9.4.0]
```

---

## Задача 4 (*)

Воспроизвести практическую часть лекции самостоятельно.

- Создать виртуальную машину.
- Зайти внутрь ВМ, убедиться, что Docker установлен с помощью команды
```
docker ps
```

---
**Решение**

```
vagrant@ubuntu-server1:~$ sudo docker ps
CONTAINER ID   IMAGE     COMMAND   CREATED   STATUS    PORTS     NAMES
```

---
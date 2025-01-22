# Ansible WebApp Deployment 

## Описание проекта

Этот проект предназначен для автоматизации развертывания веб-приложения с использованием Ansible. Он включает в себя настройку веб-сервера (Nginx), базы данных (MySQL), а также настройку создания бэкапа. Проект состоит из нескольких ролей Ansible, каждая из которых отвечает за определенную часть инфраструктуры.


## Структура проекта
```
ansible-webapp-deployment/
├── roles/
│   ├── web_server/      # Роль для установки и настройки веб-сервера
│   ├── database/        # Роль для установки и настройки базы данных
│   └── backup/          # Роль для резервного копирования базы данных
├── inventory/
│   ├── hosts.ini        # Инвентарь для указания серверов
│   └── group_vars/      # Переменные групп
├── playbook_main.yml
├── README.md            # Документация проекта
└── ansible.cfg          # Конфигурация Ansible
```

## Использование

**1. Клонируйте репозиторий:**

```
git clone https://github.com/Reycoon/ansible-webapp-deployment.git

cd ansible-webapp-deployment
```

**2. Настройте инвентарь в inventory/hosts.ini и параметры в group_vars в соответствии с вашей инфраструктурой.**

**3. Запустите playbook:**

```
ansible-playbook playbook_main.yml -i inventory/hosts.ini
```

## Роли

* *web_server* — установка и настройка Nginx.
* *database* — установка и настройка MySQL.
* *backup* — настройка резервного копирования базы данных.

Каждой Описание роли находится в соответствующем каталоге. 


<p>
</br>
  <img src="https://img.shields.io/badge/ansible-%231A1918.svg?style=for-the-badge&logo=ansible&logoColor=white">
  <img src="https://img.shields.io/badge/nginx-%23009639.svg?style=for-the-badge&logo=nginx&logoColor=white">
  <img src="https://img.shields.io/badge/mysql-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white">
</p>

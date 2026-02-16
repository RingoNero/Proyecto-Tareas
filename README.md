# 📝 Sistema de Gestión de Tareas Colaborativo

Este es un sistema  de gestión de tareas desarrollado con **CodeIgniter**. Permite a los usuarios organizar su trabajo personal, desglosar tareas complejas y colaborar con otros miembros en tiempo real.

## 🚀 Características Principales

* **Autenticación de Usuarios:** Registro e inicio de sesión seguro para cada usuario.
* **Gestión de Tareas:** Creación, edición y eliminación de tareas principales.
* **Subtareas:** Capacidad de desglosar una tarea en pasos más pequeños para un mejor seguimiento.
* **Colaboración:** Sistema de invitaciones para que otros usuarios registrados puedan visualizar y gestionar tareas compartidas.
* **Estados de Tarea:** Control de flujo mediante estados: `Pendiente`, `En Proceso` y `Completado`.
* **Fechas Límite:** Configuración de *deadlines* para asegurar el cumplimiento de objetivos.

## 🛠️ Tecnologías Utilizadas

* **Backend:** PHP (Framework CodeIgniter)
* **Base de Datos:** MySQL
* **Frontend:** HTML5, CSS3 (Bootstrap para el diseño responsivo)

## 📦 Instalación

1. Clona el repositorio:
   ```bash
   git clone [https://github.com/RingoNero/Proyecto-Tareas.git](https://github.com/RingoNero/Proyecto-Tareas.git)

2.instalar las dependencias de codeigniter con composer install en la carpeta del proyecto clonado

3.Importa la base de datos database.sql en tu servidor local (XAMPP/WAMP).

4.Configura el archivo app/Config/Database.php con tus credenciales.
   


# CodeIgniter 4 Application Starter

## What is CodeIgniter?

CodeIgniter is a PHP full-stack web framework that is light, fast, flexible and secure.
More information can be found at the [official site](https://codeigniter.com).

This repository holds a composer-installable app starter.
It has been built from the
[development repository](https://github.com/codeigniter4/CodeIgniter4).

More information about the plans for version 4 can be found in [CodeIgniter 4](https://forum.codeigniter.com/forumdisplay.php?fid=28) on the forums.

You can read the [user guide](https://codeigniter.com/user_guide/)
corresponding to the latest version of the framework.

## Installation & updates

`composer create-project codeigniter4/appstarter` then `composer update` whenever
there is a new release of the framework.

When updating, check the release notes to see if there are any changes you might need to apply
to your `app` folder. The affected files can be copied or merged from
`vendor/codeigniter4/framework/app`.

## Setup

Copy `env` to `.env` and tailor for your app, specifically the baseURL
and any database settings.

## Important Change with index.php

`index.php` is no longer in the root of the project! It has been moved inside the *public* folder,
for better security and separation of components.

This means that you should configure your web server to "point" to your project's *public* folder, and
not to the project root. A better practice would be to configure a virtual host to point there. A poor practice would be to point your web server to the project root and expect to enter *public/...*, as the rest of your logic and the
framework are exposed.

**Please** read the user guide for a better explanation of how CI4 works!

## Repository Management

We use GitHub issues, in our main repository, to track **BUGS** and to track approved **DEVELOPMENT** work packages.
We use our [forum](http://forum.codeigniter.com) to provide SUPPORT and to discuss
FEATURE REQUESTS.

This repository is a "distribution" one, built by our release preparation script.
Problems with it can be raised on our forum, or as issues in the main repository.

## Server Requirements

PHP version 8.1 or higher is required, with the following extensions installed:

- [intl](http://php.net/manual/en/intl.requirements.php)
- [mbstring](http://php.net/manual/en/mbstring.installation.php)

> [!WARNING]
> - The end of life date for PHP 7.4 was November 28, 2022.
> - The end of life date for PHP 8.0 was November 26, 2023.
> - If you are still using PHP 7.4 or 8.0, you should upgrade immediately.
> - The end of life date for PHP 8.1 will be December 31, 2025.

Additionally, make sure that the following extensions are enabled in your PHP:

- json (enabled by default - don't turn it off)
- [mysqlnd](http://php.net/manual/en/mysqlnd.install.php) if you plan to use MySQL
- [libcurl](http://php.net/manual/en/curl.requirements.php) if you plan to use the HTTP\CURLRequest library

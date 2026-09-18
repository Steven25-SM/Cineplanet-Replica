# CINEPLANET-REPLICA

Proyecto web desarrollado con **PHP + MySQL/MariaDB + Bootstrap**.

## 1. Requisitos

Instalar:

* **XAMPP** → Apache + MySQL/MariaDB
* **Visual Studio Code**
* **Composer** → necesario para las dependencias PHP

### Extensiones recomendadas de VS Code

* **PHP Intelephense** → autocompletado y análisis de PHP
* **PHP Server** → opcional para proyectos PHP simples, pero este proyecto se ejecuta con **XAMPP**
* **MySQL** / **Database Client** → opcional para administrar la BD desde VS Code

---

## 2. Clonar o colocar el proyecto

El proyecto debe estar dentro de:

```text
C:\xampp\htdocs\Cineplanet-Replica
```

Abrir **esa carpeta exacta** en VS Code.

> Importante: editar la copia que está dentro de `htdocs`, porque esa es la que ejecuta Apache.

---

## 3. Iniciar XAMPP

Abrir XAMPP y activar:

```text
Apache  → Start
MySQL   → Start
```

---

## 4. Crear la base de datos

Entrar a:

```text
http://localhost/phpmyadmin
```

Crear/importar la base de datos:

```text
cineplanet
```

Importar el archivo:

```text
cineplanet.sql
```

El proyecto utiliza:

```text
Host: localhost
Usuario: root
Contraseña: (vacía)
Base de datos: cineplanet
```

---

## 5. Instalar dependencias PHP

Desde la carpeta del proyecto:

```bash
composer install
```

Esto instala las dependencias definidas en `composer.json`, incluyendo:

```text
PHPMailer
```

No es necesario ejecutar `composer update`.

---

## 6. Ejecutar

Con Apache y MySQL activos:

```text
http://localhost/Cineplanet-Replica/index.php
```

También puede accederse mediante:

```text
http://localhost/Cineplanet-Replica/
```

---

## 7. Estructura importante

```text
Cineplanet-Replica/
├── db/
├── img/
├── includes/
├── media/
├── uploads/
├── vendor/
├── composer.json
├── composer.lock
├── config.php
├── index.php
└── ...
```

### ⚠️ Importante

No mover el proyecto fuera de:

```text
C:\xampp\htdocs\
```

si se quiere ejecutarlo directamente mediante Apache/XAMPP.

---

## Stack

* PHP
* MySQL / MariaDB
* Apache
* Bootstrap
* PHPMailer
* Composer
* HTML / CSS / JavaScript

# PhpMyAdmin Ready

Dépôt d'utilisation de phpmyadmin prêt à l'emploi.

## 1 - Pré-requis

- Environnement Php :
	- Composer: 2.8.9
	- Php: 8.4.7
		- Zend Engine: v4.4.7
			- with Xdebug: v3.4.1
			- with Zend OPcache: v8.4.7
- Environnement JS :
	- Node: 22.17.1
	- Npm: 10.9.2

## 2 - Chargement de composer

```
composer install && npm install
```

## 3 - Configuration du fichier `config.inc.php`

### 3.1 - Blowfish Secret

Remplacer la clé `blowfish_secret` par une nouvelle chaîne de caractère quelconque.

```
$cfg['blowfish_secret'] = ']fsTicMkQ.UuY1-8exM9Hded8}iw=C:H';
```

### 3.2 - Ip du serveur MySQL

Remplacer l'ip du serveur MySQL par celui du votre.

```
$cfg['Servers'][$i]['host'] = 'localhost';
```

### 3.3 - IDs de connexion à MySQL

Remplacer les IDs `root ` par l'identifiant et le mot de passe de votre serveur MySQL.

```
$cfg['Servers'][$i]['user'] = 'root';
$cfg['Servers'][$i]['password'] = 'root'; 
```

## 4 - Démarrage

```
php -S localhost:8000
```

Accès : [http://localhost:8000](http://localhost:8000)
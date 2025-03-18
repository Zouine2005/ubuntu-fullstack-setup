# Ubuntu Fullstack Setup Guide

## 👨‍💻 Description
Un guide complet pour installer et configurer votre environnement de développement sous **Ubuntu** avec **PHP 8+, Laravel, React.js, Node.js, MySQL, et Docker**.

---

## 🔧 1. Mise à jour d'Ubuntu
```bash
sudo apt update && sudo apt upgrade -y
```

## 🔧 2. Installer PHP 8.3 et ses extensions
```bash
sudo apt install php php-cli php-mbstring php-xml php-curl php-mysql php-sqlite3 php-zip unzip curl -y
php -v
```

## 🔧 3. Installer Composer
```bash
curl -sS https://getcomposer.org/installer | php
sudo mv composer.phar /usr/local/bin/composer
composer -V
```

## 🔧 4. Installer Laravel
```bash
composer create-project laravel/laravel nom_du_projet
```

## 🔧 5. Installer Node.js et NPM
```bash
sudo apt install nodejs npm -y
node -v
npm -v
```

## 🔧 6. Mettre à jour NPM si besoin
```bash
sudo npm install -g npm@latest
```

## 🔧 7. Installer React.js (Create React App)
```bash
npx create-react-app nom_du_projet_react
```

## 🔧 8. Installer MySQL / MariaDB
```bash
sudo apt install mysql-server -y
sudo mysql_secure_installation
```

## 🔧 9. Configurer .env de Laravel
```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=nom_de_la_base
DB_USERNAME=root
DB_PASSWORD=motdepasse
```

## 🔧 10. Installer et configurer Docker (facultatif)
```bash
sudo apt install docker.io -y
sudo systemctl start docker
sudo systemctl enable docker
sudo usermod -aG docker $USER
```

## 🔧 11. Commandes utiles Laravel
```bash
php artisan serve
php artisan migrate
php artisan cache:clear
```

## 🔧 12. Commandes utiles React
```bash
cd nom_du_projet_react
npm start
```

---

## 🌟 Bonus : Générer la clé d'application Laravel
```bash
php artisan key:generate
```

## 🔧 Vider le cache Laravel
```bash
php artisan cache:clear
```

---

## 🌐 Créé par : Zouine
*Feel free to fork, star, and contribute 👍*


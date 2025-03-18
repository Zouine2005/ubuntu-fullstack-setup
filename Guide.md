# Ubuntu Fullstack Setup Guide 🚀

## 👨‍💻 Description
A complete guide to install and configure your development environment on **Ubuntu** with **PHP 8+, Laravel, React.js, Node.js, MySQL, and Docker**.

---

## 🔧 1. Update Ubuntu
```bash
sudo apt update && sudo apt upgrade -y
```

## 🔧 2. Install PHP 8.3 and Extensions
```bash
sudo apt install php php-cli php-mbstring php-xml php-curl php-mysql php-sqlite3 php-zip unzip curl -y
php -v
```

## 🔧 3. Install Composer
```bash
curl -sS https://getcomposer.org/installer | php
sudo mv composer.phar /usr/local/bin/composer
composer -V
```

## 🔧 4. Install Laravel
```bash
composer create-project laravel/laravel project_name
```

## 🔧 5. Install Node.js and NPM
```bash
sudo apt install nodejs npm -y
node -v
npm -v
```

## 🔧 6. Upgrade NPM (Optional)
```bash
sudo npm install -g npm@latest
```

## 🔧 7. Install React.js (Create React App)
```bash
npx create-react-app react_project_name
```

## 🔧 8. Install MySQL / MariaDB
```bash
sudo apt install mysql-server -y
sudo mysql_secure_installation
```

## 🔧 9. Configure Laravel .env for MySQL
```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=your_database_name
DB_USERNAME=root
DB_PASSWORD=your_password
```

## 🔧 10. Install and Configure Docker (Optional)
```bash
sudo apt install docker.io -y
sudo systemctl start docker
sudo systemctl enable docker
sudo usermod -aG docker $USER
```

## 🔧 11. Useful Laravel Commands
```bash
php artisan serve
php artisan migrate
php artisan cache:clear
```

## 🔧 12. Useful React Commands
```bash
cd react_project_name
npm start
```


---

## 🌐 Created by: Zouine
*Feel free to fork, star ⭐, and contribute 👍*

---



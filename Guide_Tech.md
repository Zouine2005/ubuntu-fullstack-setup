# Ubuntu Fullstack Setup Guide 🚀

## 👨‍💻 Description
A complete guide to install and configure your development environment on **Ubuntu** with **PHP 8+, Laravel, MySQL,Node.js,MongoDB ,React.js,  and Docker**.

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

## 🔧 4. Install phpMyAdmin
```bash
sudo apt install apache2 -y
sudo systemctl start apache2
sudo systemctl enable apache2
```
Visit http://localhost to check if Apache is running.

---

## 🔧 3. Install phpMyAdmin
```bash
sudo apt install phpmyadmin -y
```
Visit http://localhost/phpmyadmin in your browser to access phpMyAdmin.

---

## 🔧 5. Install Composer
```bash
curl -sS https://getcomposer.org/installer | php
sudo mv composer.phar /usr/local/bin/composer
composer -V
```
---

## 🔧 6. Install Laravel
```bash
composer create-project laravel/laravel project_name
```
---

## 🔧 7. Install MySQL 
```bash
sudo apt install mysql-server -y
sudo mysql_secure_installation
```

## 🔧 8. Start Mysql Service
```bash
sudo systemctl start mysql
sudo systemctl enable mysql
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

## 🔧 10. Useful Laravel Commands
```bash
php artisan serve
php artisan migrate
php artisan cache:clear
```

## 🔧 11. Install Node.js and NPM
```bash
sudo apt install nodejs npm -y
node -v
npm -v
```

## 🔧 12. Upgrade NPM (Optional)
```bash
sudo npm install -g npm@latest
```

## 🔧 13. Install MongoDB
```bash
wget -qO - https://www.mongodb.org/static/pgp/server-7.0.asc | sudo apt-key add -
echo "deb [ arch=amd64,arm64 ] https://repo.mongodb.org/apt/ubuntu $(lsb_release -cs)/mongodb-org/7.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-7.0.list
sudo apt update
sudo apt install -y mongodb-org
```

## 🔧 14. Start MongoDB Service
```bash
sudo systemctl start mongod
sudo systemctl enable mongod
```

## 🔧 15. Install React.js (Create React App)
```bash
npx create-react-app react_project_name
```

## 🔧 16. Useful React Commands
```bash
cd react_project_name
npm start
```

## 🔧 17. Install and Configure Docker 
```bash
sudo apt install docker.io -y
sudo systemctl start docker
sudo systemctl enable docker
sudo usermod -aG docker $USER
```


---

## 🌐 Created by: Zouine
*Feel free to fork, star ⭐, and contribute 👍*

---





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

## 🔧 5. Install MySQL 
```bash
sudo apt install mysql-server -y
sudo mysql_secure_installation
```

## 🔧 6. Start MongoDB Service
```bash
sudo systemctl start mysql
sudo systemctl enable mysql
```

## 🔧 7. Configure Laravel .env for MySQL
```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=your_database_name
DB_USERNAME=root
DB_PASSWORD=your_password
```

## 🔧 8. Useful Laravel Commands
```bash
php artisan serve
php artisan migrate
php artisan cache:clear
```

## 🔧 9. Install Node.js and NPM
```bash
sudo apt install nodejs npm -y
node -v
npm -v
```

## 🔧 10. Upgrade NPM (Optional)
```bash
sudo npm install -g npm@latest
```

## 🔧 11. Install MongoDB
```bash
wget -qO - https://www.mongodb.org/static/pgp/server-7.0.asc | sudo apt-key add -
echo "deb [ arch=amd64,arm64 ] https://repo.mongodb.org/apt/ubuntu $(lsb_release -cs)/mongodb-org/7.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-7.0.list
sudo apt update
sudo apt install -y mongodb-org
```

## 🔧 12. Start MongoDB Service
```bash
sudo systemctl start mongod
sudo systemctl enable mongod
```

## 🔧 13. Install React.js (Create React App)
```bash
npx create-react-app react_project_name
```

## 🔧 14. Useful React Commands
```bash
cd react_project_name
npm start
```

## 🔧 15. Install and Configure Docker 
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





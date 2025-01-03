# Web Requests cURL Lesson Demo

This is a simple PHP applications created as part of the **Web Requests** lessons. It demonstrates the use of cURL for sending requests and receiving responses. When accessed through a regular browser, it displays a message asking you to open it with cURL. When accessed using cURL, it shows a congratulatory message.

For further lesson follow-up, visit our channel: [Bad Rebbit](https://t.me/Bad_Rabbit_Team)

## Description

This page is designed to be a fun and educational demonstration of how to interact with a web server using the cURL command line tool. The page behaves differently depending on whether it's accessed via a browser or via cURL.

- **When accessed via a browser**: The page shows the message "Come on, open it with cURL to see the real magic!".
- **When accessed via cURL**: The page shows the message "Congratulations! You nailed the lesson like a pro!".

## How to Run the Application

To run this application, follow these simple steps:

### 1. Clone the Repository

First, clone this repository to your local machine:

```bash
git clone https://github.com/kerolos000/web_requests.git
```

### 2. Setup Apache Server with PHP

Make sure you have a web server like Apache installed with PHP support. You can use **XAMPP** for Windows or **LAMP** for Linux.

#### For Linux:

Install Apache and PHP:

```bash
sudo apt update
sudo apt install apache2 php libapache2-mod-php
```

After installation, start Apache:

```bash
sudo systemctl start apache2
```

#### For Windows:

Download and install **XAMPP** from [here](https://www.apachefriends.org/index.html), then start the Apache server from the XAMPP control panel.

### 3. Place the `index.php` File

After cloning the repository, place the `index.php` file inside the web server's root directory.

- For **XAMPP** on Windows, the root directory is `C:\xampp\htdocs`.
- For **LAMP** on Linux, the root directory is `/var/www/html`.

### 4. Access the Page

- Open your browser and navigate to:

```text
http://localhost/index.php
```

You will see the message:  
*"Come on, open it with cURL to see the real magic!"*

- Now, open a terminal and use cURL to access the same page:

```bash
curl http://localhost/index.php
```

You will see the message:  
*"Congratulations! You nailed the lesson like a pro!"*

## Troubleshooting

- **Apache not starting?**  
Make sure the Apache service is running. On Linux, use the command:  
```bash
sudo systemctl start apache2
```

- **PHP not working?**  
Ensure PHP is properly installed and configured with Apache. You can test PHP functionality by creating a simple `info.php` file with the following content:

```php
<?php
phpinfo();
?>
```

Then access it via `http://localhost/info.php` in your browser.

---

Enjoy experimenting with PHP and cURL as part of the **Web Requests** course! 🎉

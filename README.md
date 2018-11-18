# Simple Web Application
Automates deployment of simple web application

## 1. Clone repository
```
  $ git clone https://github.com/amrutja26/simple_web_application.git
  $ cd simple_web_application
```

## 2. Upgrade zlib version to be compatible with mysql-5.6.42
mysql community release requires zlib 1.2.11+ now as per https://dev.mysql.com/doc/relnotes/mysql/5.6/en/news-5-6-42.html
```
 $ ansible-playbook upgrade_zlib.yml -i inventory
```
## 3. Install web application requirements and deploy the application
```
  $ ansible-playbook playbook.yml -i inventory
```

**Note: Please adjust the inventory file setting as per your environment before running ansible-playbook**

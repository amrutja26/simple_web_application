Automates deployment of simple web application

# Clone repository
$ git clone https://github.com/amrutja26/simple_web_application.git
$ cd simple_web_application

# Upgrade zlib version to be compatible with mysql-5.6.42
# mysql community release requires zlib 1.2.11+ now.
# https://dev.mysql.com/doc/relnotes/mysql/5.6/en/news-5-6-42.html

$ ansible-playbook upgrade_zlib.yml -i inventory

# Install web application requirements and deply the web application
$ ansible-playbook playbook.yml -i inventory

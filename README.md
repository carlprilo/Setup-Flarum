# Set up [Flarum](https://flarum.org/docs/install.html#server-requirements).
## Environment 
1. Ubuntu 16.04
2. PHP 7.1
3. Apache2
4. MySQL 5.6

## 1. Environment Preparation

### Ⅰ· Apache
` $ sudo apt-get update`

`$ sudo apt-get install apache2`

### Ⅱ· PHP7.1 & Extention
` $sudo apt-get install -y software-properties-common`

` $sudo add-apt-repository -y ppa:ondrej/php`

` $sudo apt-get update`

` $sudo apt-get install -y php7.1`
 
` $sudo apt-get install -y php7.1-curl`

` $sudo apt-get install -y php7.1-dom`

` $sudo apt-get install -y php7.1-gd `

` $sudo apt-get install -y php7.1-json `

` $sudo apt-get install -y php7.1-mysql `

` $sudo apt-get install -y php7.1-mbstring  `

` $sudo apt-get install -y php7.1-zip `

` $sudo apt-get install -y php7.1-tokenizer`

### Ⅲ· MySQL
` $sudo apt-get install mysql-server mysql-client`

### Ⅳ· [Composer](https://getcomposer.org/)
` $php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"`

` $php -r "if (hash_file('sha384', 'composer-setup.php') === 'a5c698ffe4b8e849a443b120cd5ba38043260d5c4023dbf93e1558871f1f07f58274fc6f4c93bcfd858c6bd0775cd8d1') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"`

` $php composer-setup.php`

` $php -r "unlink('composer-setup.php');"`

Move the _composer.phar_ right in the working drectory to /usr/local/bin/

`$mv ./composer.phar  /usr/local/bin/composer`

Try `$composer` in your teminal to test.

## 2. Install Flarum
Reference to the offcial [documention](https://flarum.org/docs/install.html#server-requirements)

## 3. Set up Mail Server.
Gmail is recommened.

Driver : _SMTP_

Username : _yourmail@gmail.com_

Password : _yourpassword_

Port : _465_

Host : _smtp.gmail.com_

Encryption : SSL

Then enable [_Less secure apps_](https://support.google.com/a/answer/6260879?hl=en) for gmail account.

## 4. Extensions

You can find various extensions of flarum [here](https://discuss.flarum.org/t/extensions).
# Send SMTP Mail
Use phpmailer class
SMTP PORT

## Dounload PHPMailer
https://github.com/PHPMailer/PHPMailer
```
PHPMailer is available on Packagist (using semantic versioning), and installation via Composer is the recommended way to install PHPMailer. Just add this line to your composer.json file:

"phpmailer/phpmailer": "~6.0"
or run

composer require phpmailer/phpmailer

Alternatively, if you're not using Composer, copy the contents of the PHPMailer folder into one of the include_path directories specified in your PHP configuration and load each class file manually:

<?php
use PHPMailer\PHPMailer\PHPMailer;
use PHPMailer\PHPMailer\Exception;

require 'path/to/PHPMailer/src/Exception.php';
require 'path/to/PHPMailer/src/PHPMailer.php';
require 'path/to/PHPMailer/src/SMTP.php';

````
## A Simple Example
```
		$mail = new PHPMailer;
		$mail->IsSMTP();			//Sets Mailer to send message using SMTP
		$mail->Host = 'ssl://smtp.gmail.com';	//Sets the SMTP hosts of your Email hosting, this for Godaddy
		$mail->Port = 465;			//Sets the default SMTP server port
		$mail->SMTPAuth = true;			//Sets SMTP authentication. Utilizes the Username and Password variables
		$mail->Username = '******@***.com';	//Sets SMTP username
		$mail->Password = '********';		//Sets SMTP password
		$mail->SMTPSecure = '';	
```
   

# Send SMTP Mail
Use phpmailer class
SMTP PORT


## Sample Code in smtp
```
$mail = new PHPMailer;
		$mail->IsSMTP();								//Sets Mailer to send message using SMTP
		$mail->Host = 'ssl://smtp.gmail.com';		//Sets the SMTP hosts of your Email hosting, this for Godaddy
		$mail->Port = 465;								//Sets the default SMTP server port
		$mail->SMTPAuth = true;							//Sets SMTP authentication. Utilizes the Username and Password variables
		$mail->Username = '******@***.com';					//Sets SMTP username
		$mail->Password = '********';					//Sets SMTP password
$mail->SMTPSecure = '';	
```
   

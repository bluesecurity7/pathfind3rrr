# Path Traversal Attack Payload List:
#Overview of Path Traversal Attacks:

Path Traversal attacks, also known as Directory Traversal attacks, are a type of security vulnerability that allows an attacker to access restricted directories and files stored outside the web root folder of a web application. This is achieved by manipulating the file paths used in the application, enabling the attacker to traverse the directory structure and gain access to sensitive files that should not be accessible. Path Traversal attacks occur when a web application fails to properly validate or sanitize user input, particularly when handling file paths. An attacker can exploit this flaw by providing crafted input that includes sequences such as ../ (dot-dot-slash), which instructs the server to navigate up the directory tree. By doing so, the attacker can access files such as configuration files, logs, or other sensitive data that may contain credentials or application secrets.

Once an attacker successfully executes a Path Traversal attack, they can read, modify, or delete sensitive files, potentially compromising the security of the entire application and the underlying server. In some cases, the attacker may even be able to execute code if they can access files containing executable scripts. To prevent Path Traversal attacks, developers should implement strict input validation, use secure coding practices, and employ access controls to restrict access to sensitive files and directories.

# Path Traversal Attack Scanner Tools:
. XSStrike


# Payload List :

../../../etc/passwd  
/etc/passwd  
....//....//....//etc/passwd  
..%252f..%252f..%252fetc/passwd  
/var/www/images/../../../etc/passwd  
../../../etc/passwd%00.png  


MySQLOldPasswordHasher
======================

Classe para criptografar as senhas utilizando o modelo da funcao old_password do mysql 4.x 
(Class to encrypt the passwords using the model of mysql 4.x  old_password function)


Como usar
======================

1. Coloque este arquivo junto do arquivo settings.py
2. Adicione o hasher ('app.hashers.MySQLOldPasswordHasher') no início da settings PASSWORD_HASERS no arquivo settings.py.

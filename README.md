MySQLOldPasswordHasher
======================

Classe para criptografar as senhas utilizando o modelo da funcao old_password do mysql 4.x.

(Class to encrypt the passwords using the model of mysql 4.x  old_password function)


Como usar
======================

1. Coloque este arquivo junto do arquivo settings.py
2. Adicione o hasher  no início da settings PASSWORD_HASERS no arquivo settings.py:


PASSWORD_HASHERS = (

    'app.hashers.MySQLOldPasswordHasher',
    
    'django.contrib.auth.hashers.BCryptPasswordHasher',
    
    'django.contrib.auth.hashers.PBKDF2PasswordHasher',
    
    'django.contrib.auth.hashers.PBKDF2SHA1PasswordHasher',
    
    'django.contrib.auth.hashers.SHA1PasswordHasher',
    
    'django.contrib.auth.hashers.MD5PasswordHasher',
    
    'django.contrib.auth.hashers.CryptPasswordHasher',
    
)


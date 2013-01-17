MySQL Old Password Hasher
======================

Classe para criptografar as senhas utilizando o modelo da função old_password do mysql 4.x no Django.

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


A função de login se mantêm sem alteração, com os métodos authenticate e authlogin normalmente.


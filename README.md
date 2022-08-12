# Самоконтроль выполненения задания

1. Где расположен файл с `some_fact` из второго пункта задания?

   group_vars/all/examp.yml


2. Какая команда нужна для запуска вашего `playbook` на окружении `test.yml`?

   ansible-playbook -i inventory/test.yml site.yml


3. Какой командой можно зашифровать файл?

   ansible-vault encrypt 


4. Какой командой можно расшифровать файл?

   ansible-vault decrypt 


5. Можно ли посмотреть содержимое зашифрованного файла без команды расшифровки файла? Если можно, то как?

   Можно, командой ansible-vault view 


6. Как выглядит команда запуска `playbook`, если переменные зашифрованы?
   
   Необходимо либо передать флаг --ask-vault-pass, чтобы при запуске ansible запросил пароль, либо передать файл с секретом через параметр --vault-password-file 


7. Как называется модуль подключения к host на windows?

   psrp - Run tasks over Microsoft PowerShell Remoting Protocol

   или

   winrm - Run tasks over Microsoft's WinRM


8. Приведите полный текст команды для поиска информации в документации ansible для модуля подключений ssh

   ansible-doc -t connection ssh


9. Какой параметр из модуля подключения `ssh` необходим для того, чтобы определить пользователя, под которым необходимо совершать подключение?
   Параметр remote_user

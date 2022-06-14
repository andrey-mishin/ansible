# Самоконтроль выполнения задания

1. Где расположен файл с `some_fact` из второго пункта задания?

**Ответ:**
```
group_vars/all/examp.yml
```

2. Какая команда нужна для запуска вашего `playbook` на окружении `test.yml`?

**Ответ:**
```
ansible-playbook site.yml -i inventory/test.yml 
```

3. Какой командой можно зашифровать файл?

**Ответ:**
```
ansible-vault encrypt group_vars/all/examp.yml
```

4. Какой командой можно расшифровать файл?

**Ответ:**
```
ansible-vault decrypt group_vars/all/examp.yml
```

5. Можно ли посмотреть содержимое зашифрованного файла без команды расшифровки файла? Если можно, то как?

**Ответ:**
```
Можно. Командой ansible-vault view <имя файла>.
```

6. Как выглядит команда запуска `playbook`, если переменные зашифрованы?

**Ответ:**
```
ansible-playbook site.yml -i inventory/prod.yml --ask-vault-pass
```

7. Как называется модуль подключения к host на windows?

**Ответ:**
```
winrm
```

8. Приведите полный текст команды для поиска информации в документации ansible для модуля подключений ssh
**Ответ:**
```
ansible-doc -t connection ssh
```

9. Какой параметр из модуля подключения `ssh` необходим для того, чтобы определить пользователя, под которым необходимо совершать подключение?

**Ответ:**
```
- remote_user
        User name with which to login to the remote server, normally set by the
        remote_user keyword.
```

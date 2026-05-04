# Задача 1: настройка posgtesql + (patroni + etcd)
 - Поднял вторую машину и сделал статический `ip` через `netplan`
 - Установил `etcd` и прописал конфиг
 - Установил `posgtgresql` создал пользователя `replicator`
 - Установил `patroni` и прописал конфиг 
 - Ноды видно но в режим `run` они не переходят
 - 
   `ETCD`
   
 <img width="1797" height="931" alt="image" src="https://github.com/user-attachments/assets/df9edbaf-628c-4d3d-bcd8-5c19d6dfb569" />
 
   `POSTGRESQL`
   
 <img width="1797" height="511" alt="image" src="https://github.com/user-attachments/assets/c2c54352-df4f-4af1-b2ee-7ec3768d5aa1" />
 
   `PATRONI`
   
 <img width="1797" height="958" alt="image" src="https://github.com/user-attachments/assets/57598fae-cf9b-4593-b6e3-121c6a162354" />
 
   `NODS`
   
 <img width="1797" height="319" alt="image" src="https://github.com/user-attachments/assets/7ef21e7a-b806-4032-b115-73ab620f337d" />

# Задача 2: запуск и настройка percona-server
 1. Установил `percona mysql` на обе машины

  <img width="1846" height="560" alt="image" src="https://github.com/user-attachments/assets/248e88d6-a876-4766-a8ca-22da59748e64" />

 2. 
  - Прописал конфиг для мастера и создал пользователя `repl` и выдал права, запомнил имя лога и позицию в таблице

   <img width="1536" height="826" alt="image" src="https://github.com/user-attachments/assets/035ec6a6-d65d-407d-8d03-95638317725e" />
   
  - Прописал конфиг для слейва и добавил хост, имя пользователя, пароль, логфайл и позицию лога в `mysql` куда ему обращаться к мастеру

    <img width="1852" height="826" alt="image" src="https://github.com/user-attachments/assets/7391358e-f178-4751-bc97-d05eb4989834" />

 3. Установил `proxysql`, зашёл админ модуль, добавил серверы в пул и настроил пользователя, затем вывел статус серверов

    <img width="1557" height="802" alt="image" src="https://github.com/user-attachments/assets/0318de61-2b00-49cb-b7b9-1d4a5865018b" />

 5. На мастере создал пользователя `backup` и выдал ему права, написал скрипт который делает бекапы с помощью утилиты `xtrabackup`

    <img width="1557" height="845" alt="image" src="https://github.com/user-attachments/assets/cc025986-bee5-4337-8a88-54340c5d05cd" />


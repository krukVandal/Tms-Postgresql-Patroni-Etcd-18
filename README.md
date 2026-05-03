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



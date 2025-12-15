# Домашнее задание к занятию "`Защита сети`" - `Фомичев Анатолий`

## Ссылка на ДЗ - https://github.com/netology-code/sdb-homeworks/blob/main/13-03.md

## Kali linux ip - 192.168.70.149
## Ubuntu 24 ip  - 192.168.70.147

### Задание 1

sudo nmap -sA 192.168.70.147  
sudo nmap -sT 192.168.70.147  
sudo nmap -sS 192.168.70.147  
sudo nmap -sV 192.168.70.147  

![alt text](https://github.com/SLzDevOps/Netology-devsec13_3/blob/main/Screenshot_616.png).  

  
Suricata на все команды сканирования, кроме sudo nmap -sA 192.168.70.147 выдает, что происходило подозрительное скарирование и классификация идет как "Потенциально опасный трафик" и "Возможна утечка информации".  

![alt text](https://github.com/SLzDevOps/Netology-devsec13_3/blob/main/Screenshot_617.png).  


В логах fail2ban нет запросов при таких сканированиях.  

![alt text](https://github.com/SLzDevOps/Netology-devsec13_3/blob/main/Screenshot_618.png).


### Задание 2  

При выполнении запроса sudo hydra -L users.txt -P pass.txt 192.168.70.147 ssh  (в настройках jail указано что 50 попыток а 3600 секунд)  была забанена машины kail linux c ip 192.168.70.149

![alt text](https://github.com/SLzDevOps/Netology-devsec13_3/blob/main/Screenshot_621.png).



  
![alt text](https://github.com/SLzDevOps/Netology-devsec13_3/blob/main/Screenshot_620.png).








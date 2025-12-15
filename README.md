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




Зашифрована директория cryptouser, создан файл для проверки  

  
![alt text](https://github.com/SLzDevOps/Netology-devsec13_3/blob/main/Screenshot_616.png).
![alt text](https://github.com/SLzDevOps/Netology-devsec13_3/blob/main/Screenshot_616.png).


Зашифрована директория командой ecryptfs-migrate-home  

  
![alt text](https://github.com/SLzDevOps/Netology-devsec13_2/blob/main/Screenshot_605.png).
![alt text](https://github.com/SLzDevOps/Netology-devsec13_2/blob/main/Screenshot_606.png).



### Задание 2


# Лабораторная работа №3
## Ход выполнения работы  
### 
**Обеспечение работоспособности протокола ICMP (для использования команды ping), при этом Windows Firewall должен быть включен для всех сетевых профилей.**   
  
1. Запускаем Group Policy Management
2. Создадим групповую политику **fw**
3. Далее переходим Computer Configuration -> Policies -> Windows Setting -> Security Settings -> Windows Defender  и включаем Firewall для всех сетевых профилей. 
![](pic/wf1.png)  
4. Далее создаем новое правило  
![](pic/wf_2.png) 
![](pic/wf_3.png) 
![](pic/wf_4.png)
5. Разрешаем ICMP запросы
![](pic/wf_5.png)   

Результат проверим на компьютере CLI. Видно, что он находится под политиками  
![](pic/wf_CLI.png)   



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

**Далее запретим анимацию при первом входе пользователей в систему на всех клиентских компьютерах домена**    
Снова создадим групповую политику Computer Configuration -> Policies -> Administrative Templates -> System -> Logon
![](pic/DC1-4_1.png)  
![](pic/DC1-4.png) 
![](pic/DC1-4_2.png)    
  
**Добавим членов группы IT в группу локальных администраторов на все компьютеры в домене**    
переходим Computer Configuration -> Policies -> Windows Setting -> Security Settings -> Restricted Groups
![](pic/DC1-1.png)  
Далее нажимаем *Add group* и добавляем *IT* в группу локальных администраторов.   
  
**Настройка домашней страницы в браузерах.**    
Для выполнения этого задания были установлены ADMX. 
![](pic/DC1-2.png)
![](pic/DC1-3_1.png)
![](pic/DC1-3.png)
![](pic/DC1-3_2.png)    
  
  ![](pic/home_page.bmp)





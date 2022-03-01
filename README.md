# ripper-wrapper

### Українською
Це скрипт для автоматизації DDoS атак на російські веб ресурси.

Скрипт обирає цілі для атаки на основі единої центральної конфігурації. Координація вибору цілей проводиться волонтерами відповідно до рекомендацій Міністерства Цифрової Трансформації України.

Атака запускається в docker-контейнерах, ізольовано від вашого локального середовища.

Дивіться подробиці використання нижче.

### English
This is a script for automation of DDoS attacks on Russian web resources.

The script picks the attack targets from a centrally managed configuration. The targets are coordinated by volunteers with accordance to the requests of the Ukrainian Ministry of Digital Transformation.

The attack runs in docker containers, isolating the executed code from your local environment.

Scroll down for English instructions.

## Ukranian (Українська)

Використовуйте VPN, налаштований на російські ІР, особливо якщо ви в Україні. З інших країн, ймовірно, без VPN буде працювати.

Встановіть докер. Це інструмент для запуску програмного коду ізольовано від всього, що відбувається на вашому комп'ютері. Найпростіший спосіб - використовувва декстопну версію: https://www.docker.com/products/docker-desktop

### Windows
0. Закачати скрипт `windows_ripper.ps1`
1. Відкрити консоль та зайти до папки зі скриптом
2. Запустити скрипт `powershell -ExecutionPolicy Bypass .\windows_ripper.ps1 -Action install -Number 10`
3. Запуск без параметрів покаже довідку `powershell -ExecutionPolicy Bypass .\windows_ripper.ps1`

### MacOS
0. Закачати скрипт `os_x_ripper.sh`
1. Відкрийте Terminal. В терміналі перейдіть до папки зі скриптом.
1. Перший запуск:  
   `os_x_ripper.sh -n 10`  
   Параметр `-n 10` задає число контейнерів. Число можна не ставити якщо потужна машина
2. Апдейт існуючого:  
   `os_x_ripper.sh -m reinstall -n 10`  
   теж можна міняти кількість контейнерів якщо відчуваєте що машина тупить
3. Зупинка атаки:  
   `os_x_ripper.sh -m stop`  
   наприклад якщо треба подзвонити кудись з відео
4. Продовження атаки:  
   `/bin/bash os_x_ripper.sh -m start`
   
   Слава Україні!
   
   
## Belarusian (Беларуская)
- Можна запускаць без параметраў (для першага запуску) - аўтаматычна ставіцца `runmode=install` і `amount=50`
- Дададзены параметр для налады колькасці кантэйнераў - напрыклад `/bin/bash os_x_ripper.sh -n 10`

### Актуальныя каманды:
1. Першы запуск:
      `/bin/bash os_x_ripper.sh -n 10`  
   лічбу ('-n 10') можна не ставіць, калі моцная машына
2. Абнаўленне ўжо існуючых кантэйнераў:
      `/bin/bash os_x_ripper.sh -m reinstall -n 10`      
   таксама можна змяняць лічбу кантэйнераў, каб адкалібраваць колькасць (напрыклад калі машына не спраўляецца)
3. Спыненне атакі:
      `/bin/bash os_x_ripper.sh -m stop`      
   калі патрэбна ўся моц кампа
4. Працягванне атакі:  
   `/bin/bash os_x_ripper.sh -m start`
   
   Слава Украіне!
   Жыве Беларусь!
   
## English

If you are in Ukraine, use a VPN with a Russian IP address. From other countries, it should be fine without a VPN.

Install docker. It is a tool for running code in a manner isolated from your local computer environment. The easiest way to get started is to use the desktop version: https://www.docker.com/products/docker-desktop

### Windows
0. Download the script`windows_ripper.ps1`
1. Open command line and go to the folder with the downloaded script
2. Run the script `powershell -ExecutionPolicy Bypass .\windows_ripper.ps1 -Action install -Number 10`
3. Run withour parameters to get short instructions `powershell -ExecutionPolicy Bypass .\windows_ripper.ps1`

### MacOS
0. Download the script `os_x_ripper.sh`
1. Run the Terminal app. In the terminal, go to the folder with the script.
2. First run:  
   `os_x_ripper.sh -n 10`  
   The parameter `-n 10` sets the number of containers. You can omit it if you have a powerful computer.
2. Update the existing setup:  
   `os_x_ripper.sh -m reinstall -n 10`  
3. Stop the attack:  
   `os_x_ripper.sh -m stop`  
   For example, if you are low on bandwidth and need to make video call.
4. Continue the attack:  
   `/bin/bash os_x_ripper.sh -m start`
   
   Glory to Ukraine!

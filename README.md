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

Встановіть докер. Це інструмент для запуску програмного коду ізольовано від всього, що відбувається на вашому комп'ютері. Найпростіший спосіб - використовувва декстопну версію: https://www.docker.com/products/docker-desktop

### Windows
0. Закачати скрипт `windows_ripper.ps1`
1. Відкрити консоль та зайти до папки зі скриптом
2. Запустити скрипт `powershell -ExecutionPolicy Bypass .\windows_ripper.ps1 -Action install -Number 10`
3. Запуск без параметрів покаже довідку `powershell -ExecutionPolicy Bypass .\windows_ripper.ps1`

### MacOS
0. Закачати скрипт `os_x_ripper.sh`
1. Відкрийте Terminal (стандартна програма на Mac OS). В терміналі перейдіть до папки зі скриптом.
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

### Windows
1. Install docker
2. Get the script windows_ripper.ps1
3. Open the command line and go to the folder with the script
4. Run the script `powershell -ExecutionPolicy Bypass .\windows_ripper.ps1 -Action install -Number 10`
5. If you run it without any parameters you'll see a simple manual message `powershell -ExecutionPolicy Bypass .\windows_ripper.ps1`

### MacOS
1. Possible to launch without parametres (first launching): silent-executing with 'runmode=install` and `amount=50`
2. You can set up amount of containers to work: `/bin/bash os_x_ripper.sh -n 10`, where n = number of containers

### List of commands (for Mac version):
1. First launch:  
   `/bin/bash os_x_ripper.sh -n 10`  
   you can skip setting the number of containers if you have a powerful computer
2. Update the existing setup:  
   `/bin/bash os_x_ripper.sh -m reinstall -n 10`  
   You may change the number of containers too if you feel like the computer is significantly slowed down.
3. Stop the attack:  
   `/bin/bash os_x_ripper.sh -m stop`  
   For example, if you are low on bandwidth and need to make video call.
4. Continue the attack:  
   `/bin/bash os_x_ripper.sh -m start`
   
   Glory to Ukraine!

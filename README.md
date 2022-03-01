# ripper-wrapper
Automation of DDoS attacks on propaganda and pro-Russian sources
## Ukranian (Українська)

### Windows
1. Поставити докер
2. Закинути скрит до папки windows_ripper.ps1
3. Відкрити консоль та зайту и папку зі скриптом
4. Запустити скрипт `powershell -ExecutionPolicy Bypass .\windows_ripper.ps1 -Action install -Number 10`
5. Запуск без параметрів покаже довідку `powershell -ExecutionPolicy Bypass .\windows_ripper.ps1`

### MacOS
1. Можна запускати без параметрів (для першого запуску) - автоматом ставить `runmode=install і amount=50`
2. Додано параметр для конфігурування кількості контейнкрів - наприклад `/bin/bash os_x_ripper.sh -n 10`

### Актуальні команди:
1. Перший запуск:  
   `/bin/bash os_x_ripper.sh -n 10`  
   число можна не ставити якщо потужна машина
2. Апдейт існуючого:  
   `/bin/bash os_x_ripper.sh -m reinstall -n 10`  
   теж можна міняти кількість контейнерів якщо відчуваєте що машина тупить
3. Зупинка атаки:  
   `/bin/bash os_x_ripper.sh -m stop`  
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

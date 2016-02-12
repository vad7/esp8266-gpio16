ESP8266 - Driver for GPIO
=========================

Номер пина = GPIO_x

<b>Схема подключения 2 кнопок к ESP-01:</b><br>
Кнопка 1 подключена к GPIO0 (Pin 3) ESP-01<br>
Кнопка 2 подключена к GPIO2 (Pin 4) ESP-01<br>

<b>[*] Вывод D0 (GPIO16) можно использовать только на чтение и запись. Прерывания не поддерживаются, использование этого выводя для шин i2c, one-wire невозможно.</b>

<b>Сборка под Windows:</b><br>
1. <a href="http://programs74.ru/get.php?file=EspressifESP8266DevKitX86">Скачайте</a> и установите компилятор и SDK.<br>
2. <a href="http://sourceforge.net/projects/mingw/files/Installer/">Скачайте</a> и установите MinGW. Запускаем mingw-get-setup.exe, в процессе установки выберите режим без GUI, то есть уберите галочку "...also install support for the graphical user interface".<br>
3. <a href="http://programs74.ru/get.php?file=EspressifESP8266DevKitAddon">Скачайте</a> (84Mb) набор моих скриптов для автоматизации установки дополнительных модулей для MinGW.<br>
4. Запустите из моего набора файл install-mingw-package.bat. Он установит основные модули для MinGW, установка должна пройти без ошибок.<br>
5. Установите <a href="http://git-scm.com/download/win">Git for Windows</a> (после установки потребуется перезагрузить компьютер).<br>
6. Запускаем консоль C:\MinGW\msys\1.0\msys.bat<br>
7. В консоле выполните:<br>
```
cd /c/Espressif/examples
git clone https://github.com/CHERTS/esp8266-gpio16
cd esp8266-gpio16
make
make flash
```

--

<b>Wiring 2 buttons to the ESP-01:</b><br>
Button 1 is connected to GPIO0 (Pin 3) ESP-01<br>
Button 2 is connected to GPIO2 (Pin 4) ESP-01<br>

Flat pin numbering: 0 - 16

<b>[*] D0(GPIO16) can only be used as gpio read/write. no interrupt supported. no pwm/i2c/ow supported.</b>

<b>Building on Windows:</b><br>
1. <a href="http://programs74.ru/get.php?file=EspressifESP8266DevKitX86">Download</a> and install compiler and SDK.<br>
2. <a href="http://sourceforge.net/projects/mingw/files/Installer/">Download</a> and install MinGW. Run mingw-get-setup.exe, the installation process to select without GUI, ie uncheck "... also install support for the graphical user interface".<br>
3. <a href="http://programs74.ru/get.php?file=EspressifESP8266DevKitAddon">Download</a> (84Mb) set my scripts to automate the installation of additional modules for MinGW.<br>
4. Run the file from my set of install-mingw-package.bat. He will establish the basic modules for MinGW, installation should proceed without error.<br>
5. Install <a href="http://git-scm.com/download/win">Git for Windows</a> (after installation to restart the computer).<br>
6. Run the console C:\MinGW\msys\1.0\msys.bat<br>
7. In the console, run:<br>
```
cd /c/Espressif/examples
git clone https://github.com/CHERTS/esp8266-gpio16
cd esp8266-gpio16
make
make flash
```

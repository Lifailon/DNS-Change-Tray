## DNS-Change-Tray - программа для быстрой смены DNS-адреса на сетевом адаптере.

Применимо для быстрой проверки преобразования имени в адрес во внешней зоне (например, при ожидании TTL обновленного адреса, или, при падении vpn-туннеля, когда dns ведет на локальные адреса), при тестирование доступности https-трафика с фильтрующим сервером, а так же для сравнения скорости ответа.

**[Скачать (DNS-Change-Tray.exe)](https://github.com/Lifailon/DNS-Change-Tray/releases/tag/DNS-Change-Tray-1.2)**.

## Вкрсия 1.2.
* Добавлен вывод при двойном клике мыши, на текущую конфигурацию выбранного сетевого интерфейса (dns, ip и шлюза).
* Добавлена кнопка Addresses, для вывода списка всех сетевых интерфейсов (ip-адреса и соответствующий им индекс).
* Увеличино с 10 до 15 DNS адресов в список меню.

![Image alt](https://github.com/Lifailon/DNS-Change-Tray/blob/rsa/Screen/IP-Configuration.jpg)
![Image alt](https://github.com/Lifailon/DNS-Change-Tray/blob/rsa/Screen/Addresses.jpg)

После запуска, если в списке присутствует адрес текущего использующегося сервера, он будет отмечен в статусе выбранного (Checked), как и после смены адреса, так же текущий адрес можно узнать двойным кликом мыши по иконке. Список адресов создается автоматически (предустановленным по умолчанию), для изменения, нажмите кнопку **Change** и добавьте адрес с новой строки (до 10 адресов), для обновления списка, нажмите кнопку **Update**.

![Image alt](https://github.com/Lifailon/DNS-Change-Tray/blob/rsa/Screen/Tray.jpg)

> Номер индекса нужного сетевого адаптера необходимо указать в первой строке файла со списком серверов (**Change**). Номер можно узнать с помощью команды: **Get-NetIPConfiguration**

![Image alt](https://github.com/Lifailon/DNS-Change-Tray/blob/rsa/Screen/Get-NetIPConfiguration.jpg)

По вопросам и предложениям **Telegram: @kup57**

## DNS-Change-Tray - программа для быстрой смены DNS-адреса на сетевом адаптере.

Применимо для быстрой проверки преобразования имени в адрес (например, при ожидании TTL обновленного адреса во внешней зоне, или, при падении vpn-туннеля, когда dns ведет на локальные адреса), при тестирование доступности https-трафика с разными серверами (фильтрующим и внешним), а так же для сравнения скорости ответа.

**[Скачать (DNS-Change-Tray.exe)](https://github.com/Lifailon/DNS-Change-Tray/releases)**.

## Версия 1.3.
* Добавлена возможность выбора индекса интерфейса в контекстном меню по выбору ip-адреса. Для этого была **реализована инициализация номера неизвестной дочерней переменной (Items)** для возможности добавления действия (Add_Click) с целью изменения конкретного значений Index в файле (событие читается только при инициализации действия, тем самым не имеет возможности задать переменные в цикле).
* Удалена кнопка Addresses. Теперь список IP-адресов всех сетевых интерфейсов отображается в меню, выбранный адрес будет отмечен (Checked).

## Версия 1.2.
* Добавлен вывод при двойном клике мыши, на текущую конфигурацию выбранного (указанного в файле) сетевого интерфейса (ip-адрес, dns и шлюза).
* Добавлена кнопка Addresses, для вывода списка всех сетевых интерфейсов (ip-адреса и соответствующий им индекс).
* Увеличино с 10 до 15 DNS адресов, выводимый в список меню.

![Image alt](https://github.com/Lifailon/DNS-Change-Tray/blob/rsa/Screen/IP-Configuration.jpg)
![Image alt](https://github.com/Lifailon/DNS-Change-Tray/blob/rsa/Screen/Addresses.jpg)

## Версия 1.1 (Release).
После запуска, если в списке присутствует адрес текущего использующегося DNS-сервера, он будет отмечен в статусе выбранного (Checked), как и после смены адреса, так же текущий адрес можно узнать двойным кликом мыши по иконке. Список адресов создается автоматически (предустановленным по умолчанию), для изменения, нажмите кнопку **Change** и добавьте адрес с новой строки (до 10 адресов), для обновления списка, нажмите кнопку **Update**.

![Image alt](https://github.com/Lifailon/DNS-Change-Tray/blob/rsa/Screen/Tray.jpg)

> Номер индекса использующегося сетевого интерфейса необходимо указать в первой строке файла со списком серверов (**Change**). Номер можно узнать с помощью команды: ` Get-NetIPConfiguration `

![Image alt](https://github.com/Lifailon/DNS-Change-Tray/blob/rsa/Screen/Get-NetIPConfiguration.jpg)

По вопросам и предложениям **Telegram: @kup57**

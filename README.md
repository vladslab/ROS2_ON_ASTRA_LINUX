# ROS2_ON_ASTRA_LINUX
Установка ROS2 на Astra Linux.

Шаг 0

Скачиваем с официального сайта Ubuntu 24.04.3 LTS
https://ubuntu.com/download/desktop

Шаг 1
Подготовка ОС, установка virt-manager

Обновляем список пакетов

`sudo apt update`

Устанавливаем виртуальную машину

`sudo apt install virt-manager`

Добавляем пользователя в группы, необходимые для работы виртальной машины

`sudo usermod -a -G livvirt,libvirt-admin,libvirt-qemu,kvm $USER`

Проверяем установку

`virt manager`

<img width="1920" height="1080" alt="Screenshot_1" src="https://github.com/user-attachments/assets/56b5be84-f2c8-48c7-aa23-d56140d2a197" /> .



Шаг 2


Установка ubuntu, настройка виртуальной машины

Нажимаем на кнопку создания виртальной машины
![Screenshot](https://github.com/user-attachments/assets/df536ada-e205-4762-bf59-624d68722c2d)  


Локальный ISO или CDROM

<img width="556" height="594" alt="Screenshot_20260207_171456" src="https://github.com/user-attachments/assets/8e474a33-4ab3-472b-9aa2-a2175738fe11" />



Выбираем ISO файл на ПК, проверяем наличие галочки "Автоматически определить по....."

<img width="672" height="612" alt="Screenshot_20260207_171528" src="https://github.com/user-attachments/assets/1d6ae9d2-867e-4841-9b48-4334f17a76de" />




<img width="810" height="574" alt="Screenshot_20260207_1716051231223" src="https://github.com/user-attachments/assets/74628ba1-3f3c-4f0c-bd38-9e12b5bb1c26" />

<img width="820" height="705" alt="Screenshot_20260207_171745" src="https://github.com/user-attachments/assets/72dba9b9-02b5-43cf-b7a6-2436cbe5a161" />

<img width="712" height="628" alt="Screenshot_20260207_171806" src="https://github.com/user-attachments/assets/9a7ed57f-dc2f-4b5a-86f5-0fe49ea38637" />

Выделяем ядра, пространство на диске и ОЗУ для ubuntu, от выбранных параметров будет зависеть быстродействие ROS2

<img width="691" height="599" alt="Screenshot_20260207_171931" src="https://github.com/user-attachments/assets/c2c6e0cb-0eb1-408c-affa-166dfa00df60" />

<img width="695" height="600" alt="Screenshot_20260207_172031" src="https://github.com/user-attachments/assets/2c1da6df-dec5-4bda-9d5b-dd1d07c943e1" />

Нажимаем "Готово" и устанвливем ОС, настраиваем её, сеть должна заработать сама, если это не так, то можно воспользовать официальной wiki https://wiki.libvirt.org/TaskNATSetupVirtManager.html

<img width="1920" height="1080" alt="Screenshot_20260207_172157" src="https://github.com/user-attachments/assets/6eb8e974-a3b8-42aa-a319-6e0bfd0ffc5e" />

<img width="1920" height="1080" alt="Screenshot_20260207_172310" src="https://github.com/user-attachments/assets/fc3c2e86-4688-4a2e-9b7f-3bd3a14d06be" />

<img width="1920" height="1080" alt="Screenshot_20260207_173414" src="https://github.com/user-attachments/assets/62017a30-384b-4347-b7ed-ad6521fdd825" />


Установку ROS2 рекомендую производить по инструкции Степана Бурмисторова https://stepik.org/lesson/1505346/step/1?unit=1525492

Готово!
<img width="1920" height="1080" alt="Screenshot_20260207_182858" src="https://github.com/user-attachments/assets/426859ef-d097-4897-86e3-43bcbfdb6565" />


При необходимости можно настроить перенаправление USB, к примеру для подключеня ESP

<img width="1278" height="237" alt="Screenshot_20260207_171111123123945" src="https://github.com/user-attachments/assets/c1158541-7673-4527-af5e-ac8b2fd88c7c" />


<img width="540" height="334" alt="Screenshot_20260207_174034" src="https://github.com/user-attachments/assets/f7ccc41c-721c-49a6-81f3-2c88b309e24d" />

















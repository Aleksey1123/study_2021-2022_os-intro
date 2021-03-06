---
## Front matter
lang: ru-RU
title: Защита лабораторной работы №5
author: Рытов Алексей Константинович НФИбд-02-21

## Formatting
toc: false
slide_level: 2
theme: metropolis
header-includes: 
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
aspectratio: 43
section-titles: true
---

# Цель работы

Ознакомление с файловой системой Linux, её структурой, именами и содержанием
каталогов. Приобретение практических навыков по применению команд для работы
с файлами и каталогами, по управлению процессами (и работами), по проверке использования диска и обслуживанию файловой системы.

# Ход работы

1. Выполнили все примеры, приведённые в первой части описания лабораторной работы.</br>

2.1.Скопировали файл /usr/include/sys/io.h в домашний каталог и назвали его
equipment.</br>

2.2. В домашнем каталоге создали директорию ~/ski.plases.</br>

2.3. Переместили файл equipment в каталог ~/ski.plases.</br>

2.4. Переименовали файл ~/ski.plases/equipment в ~/ski.plases/equiplist.</br>

---

2.6. Создали каталог с именем equipment в каталоге ~/ski.plases.</br>

2.7. Переместили файлы ~/ski.plases/equiplist и equiplist2 в каталог
~/ski.plases/equipment.</br>

2.8. Создали и переместили каталог ~/newdir в каталог ~/ski.plases и назвали
его plans.

3. Определили опции команды chmod, необходимые для того, чтобы присвоить перечисленным ниже файлам выделенные права доступа.</br>
3.1. drwxr--r-- ... australia</br>

3.2. drwx--x--x ... play</br>

3.3. -r-xr--r-- ... my_os</br>

3.4. -rw-rw-r-- ... feathers


4.1. Просмотрели содержимое файла /etc/password.

---

4.2. Скопировали файл ~/feathers в файл ~/file.old.</br>

4.3. Переместили файл ~/file.old в каталог ~/play.</br>

4.4. Скопировали каталог ~/play в каталог ~/fun.

4.6 - 4.8 Лишили владельца файла ~/feathers права на чтение. Попытались просмотреть файл командой cat. В итоге нав выдало ошибку. Попробовав скопировать файл ~/feathers мы также получили в консоли ошибку.</br>

4.9. Дали владельцу файла ~/feathers право на чтение.</br>

4.10. Лишили владельца каталога ~/play права на выполнение.</br>

4.11. Попытались перейти в каталог ~/play. Нам вывело ошибку.</br>

4.12. Дали владельцу каталога ~/play право на выполнение.


5. Использовали команду man для команд mount, fsck, mkfs, kill.

# Результат работы

Мы ознакомились с файловой системой Linux, её структурой, именами и содержанием
каталогов. Приобрели практические навыки по применению команд для работы
с файлами и каталогами, по управлению процессами, по проверке использования диска и обслуживанию файловой системы.
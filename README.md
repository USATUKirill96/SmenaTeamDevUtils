# Инструменты разработчиков

# Содержание

1. [Oh My Zsh](#ohmyzsh)
   1. [Плагины](#plugins)
   2. [Темы](#themes)
2. [RipGrep](#ripgrep)
3. [FZF](#fzf)
4. [Bat](#bat)
5. [LSD](#lsd)
6. [Tmux](#tmux)
6. [Flameshot](#flameshot)
6. [Guake terminal](#guake)
6. [KeePassXC/Bitwarden](#password)
6. [Obsidian](#obsidian)

## Oh My Zsh <a id="ohmyzsh"></a>

![Oh My Zsh](https://camo.githubusercontent.com/4db3e4069e59f51d03dd3e7fa5e89ab8fb95c9f4acda36cd5bfdf58d95269d92/68747470733a2f2f6f686d797a73682e73332e616d617a6f6e6177732e636f6d2f6f6d7a2d616e73692d6769746875622e706e67)

> **Oh My Zsh will not make you a 10x developer...but you may feel like one.**

[Github](https://github.com/ohmyzsh/ohmyzsh)

*Фреймворк для оболочки командной строки [zsh](https://www.zsh.org/). Предоставляет множество возможностей для оптимизации рабочего окружения.*



### Возможности:

- Кастомные темы для терминала
- Огромное количество крутых плагинов для командной строки [тысячи их](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins)

- Возможность прописать кастомные алиасы, делиться конфигами с другими

- Интегрируется со множеством приложений ниже

  

## Плагины Oh My Zsh <a id="plugins"></a>
### git

![image-20220218115011350](/home/aaron/code/SmenaTeamDevUtils/pictures/example)

[Github](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/git)

*Плагин для работы с гитом. Добавляет сокращения команд, текущую ветку и количество застейдженных/измененных/удаленных файлов*

- Сокращает время работы с ветками
- Спасает от ошибок, когда` что-то было случайно изменено/ удалено/ не добавлено в коммит

### zsh-autosuggestions

![image-20220216180003383](pictures/image-20220216180003383.png)

[Github](https://github.com/zsh-users/zsh-autosuggestions)

*Автоматическое продление команды на основе вашей истории*

- Супер полезная штука для длинных команд плейбуков
- Часто избавляет от необходимости пилить алиасы

### ZSH Auto-Notify

![image-20220216180505677](pictures/image-20220216180505677.png)

[Github](https://github.com/MichaelAquilina/zsh-auto-notify)

*Присылает уведомление когда долго выполняющаяся команда завершает свою работу.*

- Полезно для операций вроде выгрузки/накатывания миграций/ сборки докер образа, когда хочется переключиться фоном на что-нибудь еще.

### zsh-history-substring-search

![image-20220216181036296](pictures/image-20220216181036296.png)

[Github](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/history-substring-search)

*Поиск по истории через вхождение подстроки*

- Введите фрагмент нужной команды и перемещайтесь по истории через нажатие стрелок вверх-вниз
- Какой там командой обновить конфига nginx?

### zsh-syntax-highlighting

![image-20220216183007665](pictures/image-20220216183007665.png)

[Github](https://github.com/zsh-users/zsh-syntax-highlighting)

*Подсветка синтаксиса в терминале*

- Поможет отловить синтаксическую ошибку в команде еще на этапе ввода

### history

![image-20220216181349717](pictures/image-20220216181349717.png)

[Github](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/history)

*Объемный поиск по истории для более сложных случаев*

- `h` вывод всей истории, сокращение для `history`
- `hs` сокращение для `history | grep`



## Темы Oh My Zsh<a id="themes"></a>

### Powerlevel10k

![Powerlevel10k](pictures/prompt-styles-high-contrast.png)

[Github](https://github.com/romkatv/powerlevel10k)

Красивая кастомизируемая тема, предоставляющая кучу полезной информации в командной строке

<<<<<<< HEAD
- Отображает текущее виртуальное окружение (у тем zsh с этим проблемы обычно да)
- Хорошо кастомизируется
- Интерактивная настройка с примерами, как будут выглядеть элементы



# RipGrep<a id="ripgrep"></a>
<img src="pictures/image-20220216183845205.png" width="880" />

<img src="pictures/image-20220216184135956.png" width="880" />


​																								*Сравнение вывода `grep` и `rg`*

[Github](https://github.com/BurntSushi/ripgrep)

*Замена поиску через grep*.

- Поиск выполняется быстрее. В репозитории проекта есть бенчмарки
- Подсветка синтаксиса при выводе
- `rg` на две буквы короче чем `grep`


# FZF<a id="fzf"></a>

# <img src="pictures/image-20220216184612173.png" width="880" />

[Github](https://github.com/junegunn/fzf)

*Инструмент для нечеткого поиска по файлам. Интегрируется с bat (об этом ниже) для подсветки синтаксиса*

- Поможет, когда не совсем понятно что искать
- Очень быстрый
- Интегрируется с вимом

<img src="pictures/vimfzf.png" alt="image-20220218122556782" width="800" />

​																							*Запуск из вима через хоткей*


# Bat<a id="bat"></a>
<img src="pictures/bat" alt="image-20220218122556782" width="800" />

[Github](https://github.com/sharkdp/bat)

*Замена `cat` с подсветкой синтаксиса,  куча интеграций с другими утилитами:*

- Отображает изменения в файлах через интеграцию с `git`
- Вывод содержимого файла и подсветка синтаксиса в `fzf`
- Подсветка синтаксиса в `RipGrep`
- Превью файлов в `find` или `fd`
- Раскрашивает странички с руководством в `man`



# LSD<a id="lsd"></a>

<img src="https://raw.githubusercontent.com/Peltoche/lsd/assets/screen_lsd.png" alt="image-20220218122556782" width="800" />

[Github](https://github.com/Peltoche/lsd)

Замена `ls` с новыми фичами

- Цвета для разных типов файлов
- Иконки
- Отображение дерева папок
- Кастомизация форматирования



# Tmux<a id="tmux"></a>

<img src="pictures/tmux.png" alt="image-20220218122556782" width="800" />

[Github](https://github.com/tmux/tmux)

Терминальный мультиплексер. Позволяет создавать в терминале сессию с разделением окна и открытием вкладок

- Запустите сессию на сервере, в сессии - долгий процесс. Подключитесь на следующий день посмотреть результат
- Подключитесь к сессии коллеги посмотреть, что он на проде мутит
- Разделите окно на несколько частей для работы в разных приложениях
- А также кастомизация через плагины и конфиги



Flameshot<a id="flameshot"></a>
=======

<img src="https://flameshot.org/img/flameshot-demo.gif" width="880" />

[Github](https://github.com/flameshot-org/flameshot)

Бесплатный кроссплатформенный инструмент с открытым исходным кодом для создания скриншотов со множеством встроенных функций, позволяющих сэкономить время. 

- После скриншота не нужно отдельно их редактировать, доступно в приложении.
- Удобный интерфейс со множеством настроек "под себя".
- Простое и интуитивно понятное использование.



## Guake Terminal<a id="guake"></a>

<img src="https://user-images.githubusercontent.com/15780903/40335223-383251d6-5d80-11e8-9d43-75ae78d59f53.gif" width="880" />

[Github](https://github.com/Guake/guake) 

Представляет собой Quake-подобный (как выпадающий терминал в игре Quake) эмулятор терминала.
Основная функция этого инструмента — вызывать терминал при нажатии на горячую клавишу.

- Скорость и удобство при открытии терминала.
- Поддерживает несколько мониторов, терминал открывается на активном.
- Настройка тем, размеров и прозрачности.




## KeePassXC/Bitwarden<a id="password"></a>
<img src="https://sts10.github.io/img/keepassxc/entry-creation.gif" width="880" />

[Github-KeePassXC](https://github.com/keepassxreboot/keepassxc) [Github-Bitwarden](https://github.com/bitwarden) 

Бесплатные менеджеры паролей с открытым исходным кодом.

Используют:

- Полное шифрование базы данных с использованием 256-битного AES.
- Имеют нескольких форматов, включая веб-интерфейс, настольные приложения, расширение браузера.
- Кроссплатформенность.




## Obsidian<a id="obsidian"></a>

<img src="https://raw.githubusercontent.com/erichalldev/obsidian-smart-random-note/master/screenshot.gif" width="880" />

[Obsidian](https://obsidian.md/) 

Приложение для ведения базы знаний, имеет большое количество плагинов для тонкой настройки.
Главной функцией является построение графов, основанных на связях ваших заметок.

- Возможность синхронизации через Git.
- Использует Markdown формат файлов.
- Есть мобильное приложение с полным функционалом десктопного.
- Из минусов, не является Open-Sourсe приложением

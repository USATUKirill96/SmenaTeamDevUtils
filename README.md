

# Инструменты разработчиков



# Содержание

1. [Oh My Zsh](#ohmyzsh)



## Oh My Zsh <a id="ohmyzsh"></a>

> **Oh My Zsh will not make you a 10x developer...but you may feel like one.**



[Github](https://github.com/ohmyzsh/ohmyzsh)

Фреймворк для оболочки командной строки [zsh](https://www.zsh.org/)

Возможности:

- Кастомные темы для терминала
- Огромное количество крутых плагинов для командной строки [тысячи их](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins)



## Плагины Oh My Zsh



### git

![image-20220216175427329](pictures/example)

[Github](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/git)

> я уже не представляю чтобы я набирал целиком гитовые команды, пользуюсь только так (c) Никита Стариков

- Показывает текущую ветку, количество застейдженных/измененных/удаленных файлов
- Добавляет сокращения вида gp=git push, gd=git diff, gl = git pull, gm = git merge, gco = git checkout




### zsh-autosuggestions 

![image-20220216180003383](pictures/image-20220216180003383.png)

[Github](https://github.com/zsh-users/zsh-autosuggestions)

Автоматическое продление команды на основе вашей истории



### ZSH Auto-Notify

![image-20220216180505677](pictures/image-20220216180505677.png)

[Github](https://github.com/MichaelAquilina/zsh-auto-notify)

Присылает уведомление когда долго выполняющаяся команда завершает свою работу. Полезно для операций вроде выгрузки/накатывания миграций/ сборки докер образа, когда хочется переключиться фоном на что-нибудь еще.



### zsh-history-substring-search

![image-20220216181036296](pictures/image-20220216181036296.png)

[Github](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/history-substring-search)

Поиск по истории через вхождение подстроки

Введите фрагмент нужной команды и перемещайтесь по истории через нажатие стрелок вверх-вниз



### zsh-syntax-highlighting

![image-20220216183007665](pictures/image-20220216183007665.png)

[Github](https://github.com/zsh-users/zsh-syntax-highlighting)

Подсветка синтаксиса в терминале



### history

![image-20220216181349717](pictures/image-20220216181349717.png)

[Github](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/history)

Объемный поиск по истории для более сложных случаев



## Темы Oh My Zsh

### Powerlevel10k

![Powerlevel10k](pictures/prompt-styles-high-contrast.png)

[Github](https://github.com/romkatv/powerlevel10k)

Красивая кастомизируемая тема, предоставляющая кучу полезной информации в командной строке



# RipGrep

![image-20220216183845205](pictures/image-20220216183845205.png)

![image-20220216184135956](pictures/image-20220216184135956.png)

Сравнение вывода `grep` и `ripGrep`

[Github](https://github.com/BurntSushi/ripgrep)

Замена поиску через grep. Почему rg? Он быстрее, чем греп, у него есть подсветка синтаксиса и он быстрее набирается на клавиатуре. В репозитории проекта сравнение производительности с другими инструментами



# FZF

![image-20220216184612173](pictures/image-20220216184612173.png)

[Github](https://github.com/junegunn/fzf)

Инструмент для нечеткого поиска по файлам. Помогает в тех случаях, когда не совсем понятно, что искать. Интегрируется с bat (об этом ниже) для подсветки синтаксиса



# Bat

![](pictures/bat)

[Github](https://github.com/sharkdp/bat)

Как cat, только bat. Вывод содержимого файла в консоль с подсветкой синтаксиса. Под куча интеграций с другими утилитами:

- Отображает изменения в файлах через интеграцию с `git`
- Вывод содержимого файла и подсветка синтаксиса в `fzf`
- Подсветка синтаксиса в `RipGrep`
- Превью файлов в `find` или `fd`
- Раскрашивает странички с руководством в `man`
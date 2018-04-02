# Java-oberon-compiler
Compiler for Oberon programming language implemented with Java, Antlr4, LLVM. A project showing students that writing compilers is fun.

## Реализуемая спецификация

https://www.inf.ethz.ch/personal/wirth/Oberon/Oberon07.Report.pdf

## Установка программного обеспечения

## Клонирование данного проекта

Перед тем, как запустить пакет необходимо его склонировать с сервера в папку на компьютере.  Делается это при помощи программы `git` (https://git-scm.com/).  Можно загрузить дополнительные пакеты, интегрирующие `git` с операционной системой или редакторами.  Хороши пример такой программы - `tortoisegit` (https://tortoisegit.org/).

```shell
$ mkdir -p ~/IdeaProjects
$ cd ~/IdeaProjects
$ git clone https://github.com/eugeneai/Java-oberon-compiler.git oberon
$ cd oberon
```
Первые две строки не относятся к клонированию, они оснащают среду.

### Компиляция и запуск проекта

Для того, чтобы скомпилировать проект надо из командной строки запустить команду сборки.

```shell
$ mvn package exec:java
```

Командная строка в Linux - дело привычное: запускаете эмулятор терминала, переходите в директорий проекта (`cd ~/IdeaProjects/oberon`). В Windows все аналогично, только запускать надо `cmd.exe` или `far.exe` (если он был установлен: https://www.farmanager.com/download.php).

Программа `mvn` предназначена для сборки проекта.  Ее установка зависит от операционной системы.  Адрес - https://maven.apache.org/download.cgi . Для обеспечения ее функционирования и запуска данного проекта необходимо установить Java версии 1.8 или раньше (больше).

Если компиляция и запуск завершились удачно, то на экране появится текст, вроде этого:

```text
code generation does not match the current runtime version 4.7.1
; Running fac(10) with JIT...
; Result: 3628800
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time: 2.930 s
[INFO] Finished at: 2018-03-20T17:58:47+08:00
[INFO] Final Memory: 22M/73M
[INFO] ------------------------------------------------------------------------
```

## Разработка

Данный проект - это проект среды разработки (IDE) JetBrains IntelliJ Idea.  По идее, если на компьютере установлена эта среда, то после клонирования она должна импортировать проект в список проектов.

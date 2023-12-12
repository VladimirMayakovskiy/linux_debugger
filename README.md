# linux_debugger

---

# Задача
Написать дебаггер для проверки и отладки программ на Linux.
Многие думают, что лучший способ найти ошибку в программе - это запихнуть кучу printf и cout в нее, и с этим трудно поспорить, но в глубине души мы уверены, что отладчики тоже достаточно полезная и интересная штука.

**Функционал**

Отладчик должен поддерживать следующие функции (подробнее см. gdb):
- run, quit и continue
- точки останова
- чтение и запись регистров и памяти
- step, next, finish
- print, list
- backtrace 

Опционально:
- info (locals/ registers / frame / break) 

Интерфейс: текстовый построчный

## Стек технологий
linux api, c/c++, GNU Debugger (gdb), другие инструменты и библиотеки, такие как ptrace, libdwarf и др.

## Распределение задач по участникам

Аделина Алимова:

- [x] найти соответствующие туториалы
- [x] прочитать найденные туториалы
- [ ] сделать обработку ввода (формат gdb)
- [ ] прочитать о DWARF Debugging format
- [ ] реализовать чтение/вывод DWARF debug info
- [ ] реализовать парсер DWARF debug info
- [ ] реализовать обработку сигналов

Александр Шлыков:

- [x] прочитать найденные туториалы
- [ ] сделать обработку breakpoints
- [ ] сделать показ/изменение регистров 
- [ ] прочитать о DWARF Debugging format
- [ ] реализовать команды step_in, step_out, step_over
- [ ] реализовать поиск символов программы
- [ ] чтение/изменение переменных
# Multithreading_pthreads.c


Funktionen:
-Erstellt 4 Threads mit pthread_create
-Jeder Thread führt eine eigene Funktion aus (func1, func2 usw.)
-Threads laufen parallel und geben jeweils 10.000 Nachrichten aus
-Verwendet pthread_join, um auf das Ende aller Threads zu warten


Kompilierung und Ausführung:-

Voraussetzungen:

-GCC- oder Clang-Compiler
-POSIX-kompatibles System (z. B. Linux oder macOS)

Kompilieren:
gcc -pthread -o printer multi_threaded_printer.c

Ausführen:
./printer

Hinweise:
-Die Ausgabe kann durcheinander erscheinen, da mehrere Threads gleichzeitig auf stdout zugreifen.
-Für synchronisierte Ausgaben kann ein pthread_mutex_t verwendet werden.

# Instalacja

## Windows

* Pobierz PHP
[32bit](https://windows.php.net/downloads/releases/php-7.2.10-nts-Win32-VC15-x86.zip)
lub
[64bit](https://windows.php.net/downloads/releases/php-7.2.10-nts-Win32-VC15-x64.zip)
* Wypakuj w wybrane przez ciebie miejsce. Zalecamy ```C:\php\```.
* Dodaj ścieżkę z wypakowaną zawartością do zmiennej środowiskowej ```PATH```
* Zrestartuj komputer albo proces `explorer.exe`
* Sprawdź czy PHP zostało poprawnie zainstalowane wpisując do linii komend `php -v`. Powinna wyświetlić się informacja o wersji PHP
* Zainstaluj [Composer](https://getcomposer.org/Composer-Setup.exe)
* Przy pomocy konsoli wykonaj komendę ```composer install``` w folderze z zadaniem
(zmień bieżący folder za pomocą komendy ```cd```)

## Linux

```
    sudo apt install php
    php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
    php -r "if (hash_file('SHA384', 'composer-setup.php') === '544e09ee996cdf60ece3804abc52599c22b1f40f4323403c44d44fdfdd586475ca9813a858088ffbc1f233e9b180f061') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
    php composer-setup.php
    php -r "unlink('composer-setup.php');"
    mv composer.phar /usr/local/bin/composer
    // W folderze z zadaniem
    composer install
  ```

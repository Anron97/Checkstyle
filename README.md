# Checkstyle
<b>Руководство по настройки Checkstyle-IDEA plugin</b>

1. Установить плагин Checkstyle-IDEA (File -> Settings -> Plugins -> Вводите в поисковую строку CheckStyle-IDEA
P.S  У кого более старые версии IDEA необходимо искать плагин в удаленных репозиториях (я не помню как точно называется)

2. После установки настраиваем конфигуряцию Checkstyle (File -> Settings -> Other Settings -> Checkstyle. 
ВАЖНО! Checkstyle version выбрать 8.0 ! Scan Scope я поставил Java soursec (including tests) (Возможно будет только Java sources).  Скачиваем файл checkstyle-idea.xml 

3. Добавляем новую конфигурации (знак "+" справа от таблицы Configuration File). Вводим Description(на свой вкус).
   Радиобаттон Use a local Checkstyle file и выбираем путь до checkstyle-idea.xml. 
   В следующем окне попросит указать значение переменной checkstyleDirectory. В колонку Value необходимо ввести АБСОЛЮТНЫЙ путь до папки 
   в которой лежит файл supressions.xml (Например /home/ITRANSITION.CORP/a.shakarov/Software/Openbank/logistic-repository/gradle/plugins/checkstyle)
   
4. Жмем next и должно быть сообщение об успешной операции (если будет лог ошибок, значит плохо)
5. В нижней панели появится таб CheckStyle. Открываем и в активной конфигурации выбираем созданую ранее конфигурацию. Пользуемся
   Сканирование можно осуществлять по файлам, модцлям или всему проекту сразу. При двойном клике на варнинг или ошибку будет осуществлен
   переход к месту этой ошибки.
   

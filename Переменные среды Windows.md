**Переменная окружения** (переменная среды, *англ. environment variable*) - текстовая переменная операционной системы, хранящяя какую-либо информацию - например, данные о настройках системы или сведения о текущем пользователе.

# Работа с переменными
В качестве примера можно привести переменную ' %APPDATA% ', которая указывает путь до папки, в которой хранятся настройки некоторых программ текущего пользователя. Обычно это 'C:\Users\ПОЛЬЗОВАТЕЛЬ\AppData\Roaming', где ПОЛЬЗОВАТЕЛЬ - это имя пользователя. Для каждой учетной записи используется свое имя пользователя. 
Чтобы каждый раз не узнавать имя учетной записи текущего пользователя и не подставлять в путь к папке 'AppData' соответствующее значение и используется переменная окружения '%APPDATA%'.
Это позволяет, к примеру, быстро открывать папку 'AppData', для этого в меню "*Пуск -> Найти*" или "*Пуск -> Выполнить*" введите '%APPDATA%' и нажмите клавишу 'Enter'.
Чтобы получить значение переменной окружения через командную строку, используется команда 'echo', например:
(![image](https://user-images.githubusercontent.com/89955834/132615316-970ba2eb-613c-4d55-bda9-d2ab62ac836d.png)
# Список переменных 
Далее приводится список основных переменных.
|**Переменная**|**Описание**|
|-|-|
|'%APPDATA%'|Возвращает используемое по умолчанию размещение данных приложений.|
|'%PROCESSOR_ARCHITECTURE%'|Архитектура процессора. Возможные варианты: 'x86', 'IA64', 'AMD64'.|
|'%USERNAME%'|Имя текущего пользователя.|
|'%CD%'|Путь к профилю текущего пользователя.|
|'%USERPROFILE%'|Путь к профилю текущего пользователя.|
|'%WINDIR%'|Каталог, в котором установлена Windows.|
|'%LOGONSERVER%'|Имя контроллера домена, использовавшегося для авторизации текущего пользователя.|
|'%HOMEPATH%'|Возвращает полный путь к основному каталогу пользователя.|
|'%DATE%'|Возвращает текущую дату. |
|'%TIME%'|Возвращает текущее время.|
|'%COMPUTERNAME%'|Имя компьютера.|
|'%TEMP%' и '%TMP%'|Возвращает временные каталоги, по умолчанию используемые приложениями, которые доступны пользователям, выполнившим вход в систему. |
|'%ROGRAMFILES%'|Путь к каталогу 'Program Files'.|
|'%PROGRAMFILES(x86)%'|Путь к каталогу 'Program Files (x86)' в 64-разрядных системах для приложений архитектуры 'x86'.|
|'%PATH%'|Указывает путь поиска исполняемых файлов.|

# Изменение переменных
Чтобы изменить значение переменной, используется команда 'SET', например:

" SET TEMP=C:\TEMP "

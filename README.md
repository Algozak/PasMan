🔐 PasMan - Secure Password Manager (v0.3.1)

PasMan — это консольный менеджер паролей на Python, построенный на принципах ООП и обеспечивающий высокий уровень безопасности для ваших локальных данных.

Getty Images
🛡️ Что нового в v0.3.1 (Security Update)

В отличие от ранних версий, PasMan теперь не просто хранит данные, а надежно защищает их:

    AES Encryption: Все пароли шифруются с использованием библиотеки cryptography (Fernet). Даже если кто-то украдет ваш JSON-файл, он увидит только бессмысленный набор символов.

    PBKDF2 Key Derivation: Ключ шифрования не хранится в коде, а генерируется на лету из вашего Мастер-пароля.

    Input Validation: Защита "от дурака". Проверка длины, состава пароля и корректности названий сервисов.

    Colorized UI: Обновленный интерфейс с ANSI-цветами и плавными задержками (time.sleep) для лучшего пользовательского опыта.

✨ Основной функционал

    Add Password: Сохранение сервиса с автоматической проверкой сложности.

    Get Password: Мгновенная дешифровка и вывод пароля.

    Show Services: Удобный список всех ресурсов.

    Delete Entry: Безопасное удаление записей.

    Master Auth: Вход в систему по хешированному паролю (SHA-256).

🛠 Технологии

    Language: Python 3.10+

    Security: cryptography (Fernet), hashlib (SHA-256).

    Storage: Encrypted JSON.

    OS: Optimized for Linux (Fedora/Ubuntu).

📦 Установка и запуск

    ---Клонируйте репозиторий:
        Bash```
            git clone https://github.com/Algozak/PasMan-Password-Manager.git
            cd PasMan-Password-Manager

        Установите зависимости:
        Bash```
            pip install cryptography

        Запустите актуальную версию:
        Bash```
            python v0.3.1.py

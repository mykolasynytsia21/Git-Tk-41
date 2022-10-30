# Звіт до роботи 4
## Тема: Віртуальні середовища
### Мета роботи: Ознайомитися з віртуальними середовищами та програмою для полегшення роботи з нми, пакетним менеджером pip та деякими бібліотеками, методами видалення та встановлення їх.

---
### Виконання роботи
- Результати виконання завданнь;
    1. Перевірив чи встановлений pip на комп'ютері
    2. Передивися які дії  можна зробити за допомогою pip. Перевірив які бібліотеки вже інстальовані на моєму компютері та вказав їх у звіті (скріншот або стрічки що вивелись); Commands:

    ```python

  install                     Install packages.
  download                    Download packages.
  uninstall                   Uninstall packages.
  freeze                      Output installed packages in requirements format.
  inspect                     Inspect the python environment.
  list                        List installed packages.
  show                        Show information about installed packages.
  check                       Verify installed packages have compatible dependencies.
  config                      Manage local and global configuration.
  search                      Search PyPI for packages.
  cache                       Inspect and manage pip's wheel cache.
  index                       Inspect information available from package indexes.
  wheel                       Build wheels from your requirements.
  hash                        Compute hashes of package archives.
  completion                  A helper command used for command completion.
  debug                       Show information useful for debugging.
  help                        Show help for commands.

    ```

 3. Будь-яку сторонню бібліотеку можна встановити на комп'ютер за допомогою pip install команди та зразу почати її використовувати, наприклад встановимо бібліотеку requests:

     ```python

    pip install requests
    python #Зайдіть в пайтон інтерпретатор
    >>> import requests
    >>> r = requests.get('https://google.com')
    >>> r.status_code
    >>> exit()

    ```

   4. Ознайомтесь які ще методи є в бібліотеці requests, та спробуйте їх використати;
   5. Даний спосіб інсталяції робить бібліотеку загальнодоступною для даної системи. Будь-яке оновлення бібліотеки буде застосоване до всіх Python проектів на Вашому комп'ютері;

   ```python
    pip show requests
    pip install requests==2.1
    pip show requests
    pip uninstall requests

   ```
   6. Вкажіть у звіті результат виконання команд
- pip show requests
   
          Name: requests Version: 2.28.1 Summary: Python HTTP for Humans. Home-page: https://requests.readthedocs.io Author: Kenneth Reitz Author-email: me@kennethreitz.org License: Apache 2.0 Location: /usr/lib/python3.10/site-packages Requires: idna, urllib3 Required-by: requests-file, tldextract

- pip install requests==2.1

         Defaulting to user installation because normal site-packages is not writeable Collecting requests==2.1 Downloading requests-2.1.0-py2.py3-none-any.whl (445 kB)   

           ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 445.3/445.3 kB 517.0 kB/s eta 0:00:00
- pip show requests

        requests Successfully installed requests-2.1.0 [bogdandev@bogdandev lab4]$ pip show requests Name: requests Version: 2.1.0 Summary: Python HTTP for Humans. Home-page: http://python-requests.org Author: Kenneth Reitz Author-email: me@kennethreitz.com License: Copyright 2013 Kenneth Reitz Location: /home/bogdandev/.local/lib/python3.10/site-packages Requires: Required-by: requests-file, tldextract

- pip uninstall requests  

        pip uninstall requests Found existing installation: requests 2.1.0 Uninstalling requests-2.1.0: Would remove:

## Робота у віртуальному середовищі 
1. Віртуальні середовища в Python - це ізольовані середовища для роботи з 'замороженою' версією Python та його бібліотек. Середовище створюється для кожного проекту окремо і буде мати ті самі характеристики в не залежності де та на якій системі буде запущено;

2. Для створення VENVта його активації виконайте команди(bash):

    ```python
    python -m venv ./my_env
    source my_env/bin/activate
    pip install requests
    deactivate
    pip show requests
    ```
3. Вкажіть у звіті що вивела остання команда та чому

        Name: requests Version: 2.28.1 Summary: Python HTTP for Humans. Home-page: https://requests.readthedocs.io Author: Kenneth Reitz Author-email: me@kennethreitz.org License: Apache 2.0 Location: /usr/lib/python3.10/site-packages Requires: idna, urllib3 Required-by: requests-file, tldextract



### Висновок: 
>   ви відповіли на всі запитання:
- :question: Що зроблено в роботі - Ознайомився з віртуальними середовищами та програмою для полегшення роботи з нми, пакетним менеджером pip та деякими бібліотеками, методами видалення та встановлення їх.;
- :question: Чи досягнуто мети роботи - Так;
- :question: Які нові знання отримано - Дізнались що таке pip;
- :question: Чи вдалось відповісти на всі питання задані в ході роботи - так, зробили всі індивідуальні завдання;
- :question: Чи вдалося виконати всі завдання - Так;
- :question: Чи виникли складності у виконанні завдання - Ні;
- :question: Чи подобається такий формат здачі роботи (Feedback) - майже;
- :question: Побажання для покращення (Suggestions) Більще легких завдань :);
---
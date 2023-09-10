**Hагрузочный тест, используя JMeter.**

✅ Хост для нагрузки: https://httpbin.org/post

✅ Метод запроса: POST

✅ Тело запроса: `{ "user": "jmeter", "ver": 2 }`

*Требования к нагрузочному тесту:*

- [ ]  параметры `vu`, `loop` и `ramp-up` должны передаваться через командную строку;
- [ ]  отчет по НТ формируется в папку web;
- [ ]  для ответов от сервера применяются проверки:
    - [ ]  статус-код == 200;
    - [ ]  в теле ответа значение поля `json.user` == 'jmeter'.
   -  Команда для запуска теста в режиме non-CUI :   jmeter -n -t HW7.jmx -l logfile_ver.txt -e -o web -Jvu=4 -Jloop=2 -Jramp-up=1
- Ссылка на файл [Apache](https://github.com/VeronikaKonovalova/VerTesting/blob/main/Apache/ApacheJMeter.jmx).

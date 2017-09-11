# lab2
## Laboratory work II

Данная лабораторная работа посвещена изучению утилит для разработки проектов

## Tasks

- [x] 1. Ознакомиться со ссылками учебного материала
- [x] 2. Выполнить инструкцию учебного материала
- [x] 3. Составить отчет и отправить ссылку личным сообщением в **Slack**
 
## Tutorial

```bash
$ export GITHUB_USERNAME=komissarovrodion21
$ export GIST_TOKEN=ca277d06ef61094eaec29925750c26645434f299
$ alias edit=nano
```

```bash
$ npm install -g gistup
```


npm http GET https://registry.npmjs.org/gistup
npm http 200 https://registry.npmjs.org/gistup
npm http GET https://registry.npmjs.org/gistup/-/gistup-0.1.3.tgz
npm http 200 https://registry.npmjs.org/gistup/-/gistup-0.1.3.tgz
npm ERR! Error: EACCES, mkdir '/usr/local/lib/node_modules'
npm ERR!  { [Error: EACCES, mkdir '/usr/local/lib/node_modules']
npm ERR!   errno: 3,
npm ERR!   code: 'EACCES',
npm ERR!   path: '/usr/local/lib/node_modules',
npm ERR!   fstream_type: 'Directory',
npm ERR!   fstream_path: '/usr/local/lib/node_modules/gistup',
npm ERR!   fstream_class: 'DirWriter',
npm ERR!   fstream_stack:
npm ERR!    [ '/usr/lib/nodejs/fstream/lib/writer.js:171:23',
npm ERR!      '/usr/lib/nodejs/mkdirp/index.js:37:53',
npm ERR!      'Object.oncomplete (fs.js:107:15)' ] }
npm ERR!
npm ERR! Please try running this command again as root/Administrator.

npm ERR! System Linux 3.4.0+
npm ERR! command "/usr/bin/nodejs" "/usr/bin/npm" "install" "-g" "gistup"
npm ERR! cwd /mnt/c/Users/Родион
npm ERR! node -v v0.10.25
npm ERR! npm -v 1.3.10
npm ERR! path /usr/local/lib/node_modules
npm ERR! fstream_path /usr/local/lib/node_modules/gistup
npm ERR! fstream_type Directory
npm ERR! fstream_class DirWriter
npm ERR! code EACCES
npm ERR! errno 3
npm ERR! stack Error: EACCES, mkdir '/usr/local/lib/node_modules'
npm ERR! fstream_stack /usr/lib/nodejs/fstream/lib/writer.js:171:23
npm ERR! fstream_stack /usr/lib/nodejs/mkdirp/index.js:37:53
npm ERR! fstream_stack Object.oncomplete (fs.js:107:15)
npm ERR!
npm ERR! Additional logging details can be found in:
npm ERR!     /mnt/c/Users/Родион/npm-debug.log
npm ERR! not ok code 0




```bash
$ cat > ~/.gistup.json <<EOF
{
  "token": "${GIST_TOKEN}"
}
EOF
```

```bash
$ cd ~
$ mkdir -p workspace/labs/projects/
$ mkdir -p workspace/labs/tasks/
$ mkdir -p workspace/labs/reports/
```

## Report

```bash
$ cd ~/workspace/labs/
$ export LAB_NUMBER=02
$ git clone https://github.com/tp-labs/lab${LAB_NUMBER} tasks/lab${LAB_NUMBER}


Клонирование в «tasks/lab02»…
remote: Counting objects: 28, done.
remote: Total 28 (delta 0), reused 0 (delta 0), pack-reused 28
Unpacking objects: 100% (28/28), done.
Проверка соединения… готово.


$ mkdir reports/lab${LAB_NUMBER}
$ cp tasks/lab${LAB_NUMBER}/README.md reports/lab${LAB_NUMBER}/REPORT.md
$ cd reports/lab${LAB_NUMBER}
$ edit REPORT.md


[ GNU nano 2.2.6                            Файл: REPORT.md                                                             
## Laboratory work II

Данная лабораторная работа посвещена изучению утилит для разработки проектов

## Tasks

- [ ] 1. Ознакомиться со ссылками учебного материала
- [ ] 2. Выполнить инструкцию учебного материала
- [ ] 3. Составить отчет и отправить ссылку личным сообщением в **Slack**

## Tutorial

```bash
$ export GITHUB_USERNAME=<имя_пользователя>
$ export GIST_TOKEN=<сохраненный_токен>
$ alias edit=<nano|vi|vim|subl>
```

```bash
$ npm install -g gistup
```

```bash
$ cat > ~/.gistup.json <<EOF
{
                                                 [ Прочитано 97 строк ]
^G Помощь           ^O Записать         ^R ЧитФайл          ^Y ПредCтр          ^K Вырезать         ^C ТекПозиц
^X Выход            ^J Выровнять        ^W Поиск            ^V СледCтр          ^U ОтмВырезк        ^T Словарь
]




$ gistup -m "lab${LAB_NUMBER}"
```


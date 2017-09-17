
## Laboratory work II

Данная лабораторная работа посвещена изучению утилит для разработки проектов

## Tasks

- [x] 1. Ознакомиться со ссылками учебного материала
- [x] 2. Выполнить инструкцию учебного материала
- [x] 3. Составить отчет и отправить ссылку личным сообщением в **Slack**
 
## Tutorial

```bash
$ export GITHUB_USERNAME=komissarovrodion21 #задаем значение переменной окружения GITHUB_USERNAME
$ export GIST_TOKEN=ca277d06ef61094eaec29925750c26645434f299 #задаем значение переменной окружения(сохраненный токкен)
$ alias edit=nano #создаем alias на редактирование файлов с помощью nano
```

```bash
$ npm install -g gistup #устанавливаем пакет gitstup глобально, т.е. на весь компьютер
```

```bash
$ cat > ~/.gistup.json <<EOF
{
  "token": "${GIST_TOKEN}"
}
EOF
```

```bash
$ cd ~ #меняем директорию
$ mkdir -p workspace/labs/projects/ #создаем каталог projects
$ mkdir -p workspace/labs/tasks/ #создаем каталог tasks
$ mkdir -p workspace/labs/reports/ #создаем каталог reports
```

## Report

```bash
$ cd ~/workspace/labs/ #меняем директорию на labs
$ export LAB_NUMBER=02 #устанавливаем значение переменной LAB_NUMBER
$ git clone https://github.com/tp-labs/lab${LAB_NUMBER} tasks/lab${LAB_NUMBER} #клонируем репозиторий
$ mkdir reports/lab${LAB_NUMBER} #создаем каталог lab${LAB_NUMBER}
$ cp tasks/lab${LAB_NUMBER}/README.md reports/lab${LAB_NUMBER}/REPORT.md #копируем README.md в REPORT.md
$ cd reports/lab${LAB_NUMBER} #меняем директорию на reports/lab${LAB_NUMBER}
$ edit REPORT.md #редактируем файл REPORT.md
$ gistup -m "lab${LAB_NUMBER}"

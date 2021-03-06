## Для Ubuntu или Debian:

Ставишь компоненты для сборки бинарников:

```
sudo apt-get update
sudo apt-get install build-essential libssl-dev curl
```

## Для Fedora:

Ставишь компилятор C++ и сборщик Make:

```
sudo yum install gcc-c++ make
```

## Общее

Остальные команды по идее общие для обеих систем (на убунте не тестировал):

Ставишь Node Version Manager (nvm)

```
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.30.2/install.sh | bash
source ~/.bashrc
```

Ставишь необходимую версию Node.js (LTS) при помощи nvm

```
nvm install 8.11.1
```

Список доступных версий Node.js можно посмотреть при помощи команды `nvm ls-remote`, список установленных версий можно c помощью команды `nvm ls`

для удобства вызова необходимой _установленной_ версии Node.js можно прописать алиас (псевдоним):

```
nvm alias default 8.11.1
```

И сделалать этот псевдоним вызываемым по умолчанию:

```
nvm use default
```

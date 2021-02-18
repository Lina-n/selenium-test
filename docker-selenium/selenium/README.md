# selenium

## 事前準備
Dockerをインストール。dockerコマンドとdocker-composeコマンドを使用。

## 使い方
### インストールと起動方法

```bash
$ git clone https://github.com/sikkimtemi/selenium
$ cd selenium
$ docker-compose up -d
```

```bash
$ docker-compose ps
    Name               Command           State           Ports
-----------------------------------------------------------------------
chrome         /opt/bin/entry_point.sh   Up      0.0.0.0:5900->5900/tcp
python         tail -f /dev/null         Up
selenium-hub   /opt/bin/entry_point.sh   Up      0.0.0.0:4444->4444/tcp
```

### 終了方法

```bash
$ docker-compose down
```


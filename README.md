# asteroids

https://aalonso.dev/blog/2021/how-to-use-gui-apps-in-wsl2-forwarding-x-server-cdj

https://vcxsrv.com/  
В конфиге поставить галочку "Disable access control" и разрешить подключения через firewall, если спросит

```bash
export DISPLAY=$(ip route|awk '/^default/{print $3}'):0.0
echo $DISPLAY # Example working output: 192.168.128.1:0.0
```
и добавить в `~/.bashrc`
Проверить можно установив x11-apps и запустив xcalc
```bash
sudo apt install x11-apps
xeyes
xcalc
```


Запуск:  
`uv run main.py`  



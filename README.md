# asteroids

https://vcxsrv.com/  
В конфиге поставить галочку "Disable access control" и разрешить подключения через firewall, если спросит

```bash
export DISPLAY=$(ip route|awk '/^default/{print $3}'):0.0
echo $DISPLAY # Example working output: 192.168.128.1:0.0
```
и добавить в `~/.bashrc`

Запуск:  
`uv run main.py`


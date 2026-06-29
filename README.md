# HA Kiosk Dashboard

## Deploy update to Pi
curl -o /config/www/kiosk.html "https://raw.githubusercontent.com/LuckyTamagotchi/ha-kiosk/master/kiosk.html?$(date +%s)"

## Push update to GitHub
cd ~/ha-kiosk
git add -A && git commit -m "update" && git push

## Entity IDs
Piano Left: light.h600b
Piano Middle: light.h600b_2
Piano Right: light.h600b_3
Cat Lamp: light.catlamp
Moonbase Lightstrip: light.moonbase_lightstrip
Moonbase Monitor 1: light.moonbase_monitor_1
Moonbase Monitor 2: light.moonbase_monitor_2
Bedroom: switch.smart_indoor_plug_socket_1

## HA URL
http://192.168.1.19:8123/local/kiosk.html


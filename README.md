## WiFi Network Adapter Configuration
```
ifconfig wlan0
nmcli d
nmcli r wifi on
nmcli d wifi list
sudo nmcli d wifi connect <SSID> password <PASSWORD>
```

## Fan Control
```
echo <SPEED (0~255)> | sudo tee /sys/devices/pwm-fan/target_pwm
```
- **0 :** fan off
- **255 :** full speed
- **Any value between 0–255 :** sets the pulse-width modulation (PWM) duty cycle for the fan

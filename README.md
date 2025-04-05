# network_check.bat

@echo off
setlocal
set TARGET=google.com

echo [!] Проверка сети до %TARGET%...
echo.

echo [+] PING тест:
ping %TARGET%
echo.

echo [+] Трассировка маршрута:
tracert %TARGET%
echo.

echo [+] Проверка DNS:
nslookup %TARGET%
echo.

echo [✓] Диагностика завершена.
pause

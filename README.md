# zabbix-openvpn
Zabbix 3.4

Скрипт мониторинга пользователей OpenVPN.

Проверяется статус инсталляций OpenVPN, использование CPU и памяти инсталляцией OpenVPN.

Проверяется статус каждого пользователя всех инсталляций OpenVPN, и их входящий\исходящий трафик.

Установка:

 * скопировать файл `openvpn` в любую директорию, на сервере с OpenVPN (по умолчанию, `/etc/zabbix/scripts/`).
	
 * файл `userparameter_openvpn.conf` скопировать в директорию `/etc/zabbix/zabbix_agentd.d/` или скопировать содержимое
   в конец файла `/etc/zabbix/zabbix_agentd.conf` и проверить пути до скрипта `openvpn`
	
 * импортировать в zabbix шаблон openvpn.xml

 * скопировать файл `sudoers-zabbix` в директорию `/etc/sudoers.d/`

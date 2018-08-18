# Шаблон мониторинга OpenVPN для Zabbix 3.4

Скрипт мониторинга пользователей OpenVPN.

Проверяется статус инсталляций OpenVPN, использование CPU и памяти инсталляцией OpenVPN.

Проверяется статус каждого пользователя всех инсталляций OpenVPN, и их входящий\исходящий трафик.

Установка:

 * скопировать директории `scripts`, zabbix_agentd.d в `/etc/zabbix/` на сервере с OpenVPN.
	
 * импортировать в zabbix шаблон `Template App Openvpn.xml`

 * скопировать файл `sudoers.d/zabbix` в директорию `/etc/sudoers.d/`. Если файл `/etc/sudoers.d/zabbix` существует, то дописать в конец: `cat sudoers.d/zabbix >> /etc/sudoers.d/zabbix`
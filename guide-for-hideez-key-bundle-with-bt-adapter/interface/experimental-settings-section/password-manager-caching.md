# Password manager caching

![](<../../../.gitbook/assets/image (55).png>)

This checkbox allows the Client app to cache password manager in memory during the session. When hardware vault is disconnected from the workstation during one Client session, its storage remains cached in the application memory. Therefore the Client does not need to load all data again each time the key is connected to the Client, the vault is ready to use instantly.

{% hint style="warning" %}
Password manager cache speeds up device connection by keeping **non-sensitive data** (e.g. account name, login, list of applications) in memory until application is restarted.

\
Account passwords, OTP and other sensitive data are **never cached** and cannot be accessed without connected device.
{% endhint %}

If you will close the Client, all cached data is removed. It means that when the application is restarted (e.g. after PC reboot) the vault storage is loaded again.

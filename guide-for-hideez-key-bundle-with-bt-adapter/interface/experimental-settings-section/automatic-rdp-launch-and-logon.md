# Automatic RDP Launch and Logon

This feature allows to automatically start RDP connection to specified workstation and automatically enter credentials if they are requested by this connection.

These features can be used independently from each other.

### **Automatic RDP Logon**

To set up automatic logon into RDP, perform the following steps:

* Open Hideez Client settings page, scroll down to ‘**Experimental**’ section and select ‘_**Automatically enter credentials into applications**_’ option\
  \
  ![](<../../../.gitbook/assets/image (114).png>)\

* Create a new or edit an existing account according to the following requirements
  * Enter remote computer name into account name field (e.g. DESKTOP-68U4A)
  * Enter remote user name into login field (e.g. User1)
  * Enter remote user password into password field
  * Click ‘Add Application’ button, scroll to the end and select ‘**automate:mstsc**’
  * Click ‘Save’ button

{% hint style="warning" %}
Then you have to restart your PC for the changes to take effect.
{% endhint %}

{% hint style="info" %}
**Note:** Hideez Client can only perform automatic credentials entry if vault is authorized and password manager storage is loaded. If password manager storage is not yet loaded, automatic credentials entry will not be performed.
{% endhint %}

If everything is configured correctly, next time when RDP prompts user to enter credentials for specified workstation, Hideez Client will try to automatically use credentials from account saved in it’s storage.

If the computer name and/or username displayed by the credentials prompt doesn’t match those saved in the password manager, automatic credentials entry will not be performed.

{% hint style="info" %}
**Note:** Currently if more than one account is saved with ‘automate:mstsc’ application, only the first one will be used, where order is determined by internal vault firmware
{% endhint %}

{% hint style="info" %}
**Note:** Due to certain technicalities, currently this feature is only implemented for the English localization of Windows
{% endhint %}

### **Automatic RDP Launch**

To configure RDP to start automatically, follow these steps:

* Open Hideez Client settings page, scroll down to ‘**Experimental**’ section and select ‘_**Automatically launch applications after storage is loaded**_’ option\
  \
  ![](<../../../.gitbook/assets/image (32).png>)\

* Create a new or edit an existing account according to the following requirements
  * Enter remote computer name into account name field (e.g. DESKTOP-68U4A)
  * Click ‘Add Application’ button, scroll to the end and select ‘**automate:mstsc**’
  * Click ‘Save’ button

If everything is configured correctly, next time when password manager finishes loading storage, Hideez Client will initiate RDP connection to the workstation using the computer name specified in the saved account.

{% hint style="info" %}
**Note:** If an instance of RDP application is already running in the current local user session, automatic RDP launch will not be performed.
{% endhint %}

{% hint style="info" %}
**Note:** Currently if more than one account is saved with ‘automate:mstsc’ application, only the first one will be used, where order is determined by internal vault firmware.
{% endhint %}

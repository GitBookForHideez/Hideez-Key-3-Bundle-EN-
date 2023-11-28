---
description: Hideez Key — Proximity settings
---

# PC locking / unlocking methods (Proximity Settings)

{% embed url="https://youtu.be/Y5pbIiUALBA" %}

Hideez Key allows you to set up locking and unlocking your PC with the proximity mechanism. Your PC will be locked when the Bluetooth signal level falls below the specified value in % and unlocked when the Bluetooth signal level exceeds the specified value in %.&#x20;

{% hint style="warning" %}
Please note that we are talking about % values, and not about absolute distances in meters. The actual distance in meters can vary in different rooms and depend on external factors (the placement of the Hideez Key, the presence of furniture and walls in the room, etc.). You need to experimentally determine the optimal parameters for yourself.
{% endhint %}

{% embed url="https://youtu.be/_dPtPQVDzGM" %}

{% hint style="warning" %}
The proximity mechanism is not very stable. The signal can constantly change (even when the key is in one place). In a few seconds, the signal level can change by 30-40 units! This is influenced by many factors: mobile network and other Bluetooth devices, etc. These are the features of the technology itself.

According to our observations, we recommend setting the intervals between the values ​​at least 40. We have chosen the optimal values: \
\- Lock - 30;\
\- Unlock - 70.
{% endhint %}

Go to the **Vault settings** section and the **Lock and Unlock** block to configure Proximity settings. Check the checkbox. The Proximity level setting appears.

<figure><img src="../../.gitbook/assets/image (148).png" alt=""><figcaption></figcaption></figure>

## Configure PC Lock by Proximity

1. Check the box next to the **Use this device** **to Lock the PC** option.&#x20;
2. Adjust with the slider or enter a numeric value in the **Lock** field.&#x20;
3. Save your changes.

![](<../../.gitbook/assets/image (203).png>)

Now, as soon as the Bluetooth signal level drops below the specified value in %, your PC will be locked.&#x20;

**This is the only configurable way to lock your PC.**

## Configure PC Unlock

1. Check the box next to the **Use this device to Unlock the PC** option.&#x20;
2. Create an account to unlock your PC. You can read more about working with this type of account [here](create-and-manage-an-account-to-unlock-your-pc.md).&#x20;
3. Select a [method to unlock your PC](configure-the-methods-of-locking-and-unlocking-the-pc-proximity-settings.md).&#x20;
4. Adjust with the slider or enter a numerical value in the **Unlock** field (only for certain unlocking methods).&#x20;
5. Save your changes.

<figure><img src="../../.gitbook/assets/image (145).png" alt=""><figcaption></figcaption></figure>

The PC Unlock account on the key can be saved even if you disable the option to unlock the PC using Hideez Key. Just click 'No' in the box that appears after unchecking 'Use this device to Unlock the PC' and saving the changes.



<figure><img src="../../.gitbook/assets/image (25).png" alt=""><figcaption></figcaption></figure>

![](<../../.gitbook/assets/image (92).png>)

### Options for unlocking your PC

#### Tap & Go

{% hint style="danger" %}
This method is available only when using Hideez Key + Hideez Dongle.
{% endhint %}

The PC will be unlocked after a short tap of the Hideez Key on the Hideez Dongle. With this unlocking method, there is no need to adjust the proximity level, because it is not used and physical contact is necessary.&#x20;

#### Wait for user activity

This is a kind of proximity unlocking. In order for the PC to be unlocked, 2 conditions must be met:&#x20;

1. the Bluetooth signal level must exceed the specified value in%&#x20;
2. the user must perform an action (mouse click / key press on the keyboard)&#x20;

This method is useful when you are often near the computer. For example, you are passing by, but you do not want it to be unlocked every time.

#### Automatic unlock

Unlocking the PC only by the proximity mechanism. As soon as the Bluetooth signal level exceeds the set value in%, your PC will be unlocked.

If there is no Hideez login option on the lock screen, please, [check if the "Hide Hideez workstation logon option" is unchecked](../interface/general-settings/logon.md).

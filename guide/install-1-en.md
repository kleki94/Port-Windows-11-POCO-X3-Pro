<img align="right" src="https://github.com/woa-vayu/src_vayu_windows/blob/main/2Poco X3 Pro Windows.png" width="350" alt="Windows 11 Running On A Poco X3 Pro">


# Running Windows on the POCO X3 Pro

## Installation

## Partitioning your device

### Prerequisites

- [Modified TWRP](../../../releases/Recoveries)

- [ADB & Fastboot](https://developer.android.com/studio/releases/platform-tools)

### Notes
> [!WARNING]  
> If you ever delete any partitions via diskpart, Windows will send a UFS command which would erase the entire UFS storage!
> 
> All your data will be erased! Backup now if needed.
> 
> Do not run the same command twice.
> 
> DO NOT REBOOT YOUR PHONE if you think you made a mistake, ask for help in the [Telegram chat](https://t.me/winonvayualt).
> 
>
> Do not run all commands at once, execute them in order!
>
> YOU CAN BREAK YOUR DEVICE WITH THE COMMANDS BELOW IF YOU DO THEM WRONG!!!

> [!IMPORTANT]
> Make sure you use the MODDED TWRP Recovery throughout this whole tutorial as we provide tools to help aid this installation process and make it as easy as possible for you.
> 
> If you dont use it and you face any errors, consider it your fault and consider yourself alone if you try asking for support as you have deferred from the main guide.

##### Flash the modified TWRP recovery
```cmd
fastboot flash recovery path\to\twrp.img
fastboot reboot recovery
```

##### Run the partitioning script

> If it asks you to run it once again, do so

> This is **optional** but you can **set custom sizes using this script**

> To set custom sizes do ```adb shell partition [TARGET WINDOWS SIZE IN GB]```

> Make sure you do not add GB at the end, just the number

```cmd
adb shell partition
```

#### Check if Android still starts
Just restart the phone, and see if Android still works


## [Next step: Installing Windows](/guide/install-2-en.md)

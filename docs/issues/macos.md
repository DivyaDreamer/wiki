---
id: macos
title: Common issues on MacOS
sidebar_label: For MacOS
slug: macos
---

### Mac: Can't assign requested address (code=49)

#### Can't assign requested address (code=49) is a bug in macOS and not an issue with CloudLAN itself.

There are two ways of fixing this issue. The first one is easier as you simply have to restart your computer. Otherwise, you can solve the problem through the terminal. If you have a cable connection, you type the following into a terminal:
```
sudo ifconfig en0 down

sudo route flush

sudo ifconfig en0 up

If you instead use WiFi, you type:

sudo ifconfig en1 down

sudo route flush

sudo ifconfig en1 up
```

Type every line separately. If asked for your password, simply type the password for your computer and not for CloudLAN.

If the command sudo route flush takes longer than 10 seconds to complete, hold down Ctrl + C.




---

:::info
:information_desk_person: **Have you any question which is not answered in this knowledge base? **
Contact us, We are here to help you. at [hello@simply5.io](mailto:hello@simply5.io) or "chat with support" from our website or inside the app
:::

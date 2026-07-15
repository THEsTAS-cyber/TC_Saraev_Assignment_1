---
title: "Connect to a virtual machine (VM)"
weight: 50
---

## How to connect to your VM

You have three options to connect to your VM:

- **SSH client** — Use PuTTY (Windows) or MobaXterm (Windows, Linux, macOS). Requires an SSH key configured during VM creation.
- **Browser** — Connect directly from your web browser (see [How to connect to your VM from the browser](#how-to-connect-to-your-vm-from-the-browser)).
- **SSH by IP** — Connect using the VM's IP address with any SSH client (see [How to see the IP of the VM](#how-to-see-the-ip-of-the-vm)).

## How to see the IP of the VM

1. On your VM dashboard, find the IP address on the right side of the page.
   ![IP Address](../../../images/IP.jpg)
2. The IP looks like this: `10.13.127.89`.
   ![IP Mini](../../../images/IP_mini.jpg)
3. If there is no IP, see the section "How to create a VM with an explicit IP" (will be updated soon).

## How to connect to your VM from the browser

1. On your VM dashboard, click the **CONNECT** button at the bottom.
   ![Connect Button](../../../images/Vm_connect_button.png)
2. Choose the connection method. To connect from the browser, click **WebConsole**.
   ![Connect Options](../../../images/Connect_choose_web.png)
3. A new browser window will open with your VM console.
   ![Web Console](../../../images/Vm_web_console.png)
4. Enter your VM **login** (see [What is my VM login](../02-details-login/)) and press Enter.
5. Enter your VM **password** and press Enter.
6. If you see the message **Login is incorrect**, you entered the wrong login or password. Try again with the correct credentials.
   ![Login Incorrect](../../../images/Login_is_incorrect.png)
7. If you successfully connected, you will see a message like **Welcome to Ubuntu...** or similar, depending on your VM operating system.
   ![Successful Login](../../../images/Succesfull_login.png)
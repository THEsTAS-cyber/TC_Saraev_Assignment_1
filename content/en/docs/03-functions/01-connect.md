---
title: "Connect to VM"
weight: 50
---
## How to connect to your virtual machine

You have several options to connect to your virtual machine:

- You can use the clients or applications for ssh connection. For example, PuTTY for Windows, or MobaXterm for Windows, Linux and Mac. But for this option you need to configure the "SSH KEY" during creating virtual machine.
- You can use the connect to your virtual machine from the browser (see below).
- Connect to your virtual machine using its IP by another software (see below).

## How to see the IP of the virtual machine

1. On the page of your virtual machine dashboard on the right side you can see the IP of your virtual machine.
   ![IP Address](../../../../images/IP.jpg)
2. The IP looks like this: `10.13.127.89`.
   ![IP Mini](../../../../images/IP_mini.jpg)
3. If there is no IP - see section "How to create a virtual machine with an explicit IP" (will be updated soon).

## How to connect to your virtual machine from the browser

1. From the page of your virtual machine dashboard, click on the "CONNECT" button on the bottom.
   ![Connect Button](../../../../images/Vm_connect_button.png)
2. Then you can choose two options to connect to your virtual machine, to connect from the browser, click "WebConsole".
   ![Connect Options](../../../../images/Connect_choose_web.png)
3. The new browser window will open with your virtual machine console.
   ![Web Console](../../../../images/Vm_web_console.png)
4. You need to write your VM login (see [What is my virtual machine login](../../03-functions/02-details-login/)) and type enter.
5. And then you need to write your VM password and type enter.
6. If you see the message like "Login is incorrect". It means that you wrote incorrect login or password. Try again with correct login and password.
   ![Login Incorrect](../../../../images/Login_is_incorrect.png)
7. If you successfully connected to your virtual machine, you can see the message "Welcome to Ubuntu..." or something else depending on your virtual machine operating system.
   ![Successful Login](../../../../images/Succesfull_login.png)

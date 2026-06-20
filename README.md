# TC_Saraev_Assignment_1

The goal of this document is to guide students, instructors, and workers of Innopolis University how to use [Innopolis VM](https://vm.innopolis.university) and create your own virtual machine within Innopolis network.

[Innopolis VM](https://vm.innopolis.university) is a website for students, instructors, and workers of Innopolis University to create their own virtual machines. The website is hosted by Innopolis University and is available to all students, instructors, and workers of the university.

Virtual machines (VMs) are a powerful tool for software development, testing, and deployment. They allow you to create isolated environments for your projects, which can help you to avoid conflicts between different software packages and to ensure that your code runs correctly in different environments, and would be accessible not only from your local machinne.

## Contents

- [TC\_Saraev\_Assignment\_1](#tc_saraev_assignment_1)
  - [Contents](#contents)
  - [How to visit Innopolis VM](#how-to-visit-innopolis-vm)
  - [How to create a new virtual machine](#how-to-create-a-new-virtual-machine)
  - [How to create a new virtual machine from gallery](#how-to-create-a-new-virtual-machine-from-gallery)
  - [How to create a new virtual machine from quick start](#how-to-create-a-new-virtual-machine-from-quick-start)
  - [How to create a subscription](#how-to-create-a-subscription)
  - [Where to find your subscriptions](#where-to-find-your-subscriptions)
  - [How to connect to your virtual machine](#how-to-connect-to-your-virtual-machine)
  - [How to see the IP of the virtual machine](#how-to-see-the-ip-of-the-virtual-machine)
  - [How to create a virtual machine with an explicit IP (will be updated soon)](#how-to-create-a-virtual-machine-with-an-explicit-ip-will-be-updated-soon)
  - [How to connect to your virtual machine from the browser](#how-to-connect-to-your-virtual-machine-from-the-browser)
  - [How to see details of the created virtual machine](#how-to-see-details-of-the-created-virtual-machine)
  - [What is my virtual machine login](#what-is-my-virtual-machine-login)
  - [Password requirements](#password-requirements)
  - [Troubleshooting](#troubleshooting)

## How to visit [Innopolis VM](https://vm.innopolis.university)

1. Open your web browser and type [Innopolis VM](https://vm.innopolis.university) in the address bar. If it the first time
2. Then you will be redirected to the SSO Innopolis University [Innopolis VM](https://sso.university.innopolis.ru/adfs/ls/?wa=wsignin1.0&wtrealm=http%3a%2f%2fazureservices%2fTenantSite&wctx=rm%3d0%26id%3dpassive%26ru%3d%252f%26cx%3d0&wct=2026-06-20T09%3a03%3a51Z). ![https://sso.university.innopolis.ru/adfs/ls/?wa=wsignin1.0&wtrealm=http%3a%2f%2fazureservices%2fTenantSite&wctx=rm%3d0%26id%3dpassive%26ru%3d%252f%26cx%3d0&wct=2026-06-20T09%3a03%3a51Z](images/sso.png)
   - If you are immediately redirected to [Innopolis VM](https://vm.innopolis.university), don't worry, more likely you are already logged in.
   - If you are not logged in, you will be prompted to enter your Innopolis University credentials (username and password). Then click on the "Login" button.
3. You will be redirected to the main page of the website ![main page of https://vm.innopolis.university](images/main_page.png)

## How to create a new virtual machine

1. At first, you need to have a subscription to the service (see [How to create a subscription](#how-to-create-a-subscription)).
2. From the main page of the website, click on the "VIRTUAL MACHINES" button in the left bar ![Main virtual Machines](images/Main_virtual_machines.png)
3. - On the page with virtual machines, click on the right arrow button ![New virtual machine](images/Virtual_machines_empty_new.png)
   - If you have already created some virtual machines, you need to click on the "New" button in the left bottom corner ![New virtual machine](images/New_main.png) And then click on the "STANDALONE VIRTUAL MACHINE" in the left bar ![New virtual machine](images/Standalone_virtual_machines.png)
4. In opened menu you can choose a template for creating a virtual machine: quick start or from gallery ![Choose template](images/VM_choose_template.png)
5. - If you choose "FROM GALLERY" click the button and see [How to create a new virtual machine from gallery]     (#how-to-create-a-new-virtual-machine-from-gallery)
   - If you choose "QUICK START" click the button and see [How to create a new virtual machine from quick start](#how-to-create-a-new-virtual-machine-from-quick-start). Then you can see the massage that your virtual machine is starting to create ![VM instance start creation](images/Started_creating_vm.png)
6. To see the details of creation - click on the "DETAILS" button ![VM instance details](images/Started_creating_vm_details.png)
7. You can see the progress of creation of your virtual machine here ![VM instance creation progress](images/Creation_details_status.png)
8. On the page with virtual machines you can see your virtual machine ![Your vm](images/VMs_vm_creating.png)
9. For some time its status will be "Creating"
10. After a while its status will change to "Running" ![Your vm](images/Vm_running.png)

## How to create a new virtual machine from gallery

1. Menu with gallery creating will open ![Gallery modal](images/Gallery_modal.png)
2. You can choose the different operating system for your virtual machine and see the details.
3. When you have chosen, click right arrow button ![Gallery modal next](images/Gallery_modal_next.png).
4. Menu with settings of your virtual machine will open ![Gallery modal settings](images/Gallery_VM_settings.png)
5. Now you need to write the name of your virtual machine into "NAME" field. Name is required.
6. Write and confirm the new password for your virtual machine.
7. If you see the red exclamation mark in the "PASSWORD" field then the condition on the password is not satisfied [Password requirements](#password-requirements). Just try another password to follow the requirements.
8. If you see the red exclamation mark in the "CONFIRM" field then the password and confirm password are not equal. Just try again to write the same password in both fields.
9. If all fields are filled correctly (you don't see any red exclamation marks) - click the "CREATE VM INSTANCE" button ![Create vm instance](images/Create_VM_instance.png)
10. "ADMNISTRATOR ACCOUNT" may be fullfilled by default and can't be changed. But in some cases you are required to write your own name inside the field ![Administrator account](images/Gallery_administrator_account_marked.png)
11. Also you can write your ssh key into the "SSH KEY" field or product key into the "PRODUCT KEY" field. This is not required, but if you want - see how to configure out ssh key [How to configure and setup SSH public keys, the right way](https://dev.to/gvelrajan/how-to-configure-and-setup-ssh-public-keys-the-right-way-23be) or product key [ProductKey (microsoft-windows-setup-userdata-productkey)](https://learn.microsoft.com/en-us/windows-hardware/customize/desktop/unattend/microsoft-windows-setup-userdata-productkey).
12. Save your password, administrator account and ssh key or product key, because you will not be able to see them again.
13. When you have filled all fields, click the right arrow button ![Create vm instance](images/Vm_settings_set.png)
14. Then you can set your virtual machine network adapter - where your vm be available ![Network adapter](images/VM_adapters.png)
15. Now you can click tick button to save your settings and create virtual machine ![Save settings](images/VM_adapters_finish.png)
16. If you want to return to the previous step - click the left arrow button

## How to create a new virtual machine from quick start

1. Menu with quick start creating will open ![Quick start form](images/Quick_start_form.png)
2. Here you need to write the name of your virtual machine into "NAME" field. Name is required.
3. Also choose the subscribtion type - depending on it you can choose different templates (operating systems) for virtual michine ![Choose subscription](images/Choose_subscription_quick.png)
4. Then choose the template (operating system) for your virtual machine ![Quick start vm template](images/Template_quick_start.png)
5. Write and confirm the new password for your virtual machine.
6. If you see the red exclamation mark in the "PASSWORD" field then the condition on the password is not satisfied [Password requirements](#password-requirements). Just try another password to follow the requirements.
7. If you see the red exclamation mark in the "CONFIRM" field then the password and confirm password are not equal. Just try again to write the same password in both fields.
8. "ADMNISTRATOR ACCOUNT" may be fullfilled by default and can't be changed. But in some cases you are required to write your own name inside the field ![Fill the admin account](images/Quick_start_admin_account.png).
9. Save your password, administrator account and ssh key or product key, because you will not be able to see them again.
10. If all fields are filled correctly (you don't see any red exclamation marks) - click the "CREATE VM INSTANCE" button ![Create vm instance](images/Create_VM_instance.png)

## How to create a subscription

1. From the main page of the website, click on the "New" button in the left bottom corner ![New](images/New_main.png)
2. The new menu will open ![New page](images/New_page.png) - click "MY ACCOUNT".
3. Click on the "ADD SUBSCRIPTION" button ![Add subscription](images/My_account_subscr.png)
4. Modal with subscription creation form will open ![Subscription creation form](images/Subscription_creation_form.png)
5. Depending on what who are you (student, instructor, worker), you will have different options for subscription creation. For example, for students, you can create a subscription for a specific course or general StudentPublic subscription. If you want a specific subscription, you need to contact IT department of Innopolis University.
6. The details of the concrete subscription type will appear on the right side of the form when you click it ![Create subscription](images/Subscription_creation_form.png)
7. When you choose the subscription type - click it and then click a tick button on the right bottom corner ![Create subscription](images/Subscription_creation_form_chosen.png)
8. Then you need to wait while the subscription is being created ![Subscription creation](images/Subscription_loading.png)
9. See the status of the subscription you can see in your account [My subscriptions](#where-to-find-your-subscriptions)
10. Some time your subscription will have the "Syncing" status. Don't worry, just wait until it will be "Active" ![Subscription syncing](images/My_sub_syncing.png)
11. After a while, your subscription will change its status to "Active" ![Subscription active](images/My_sub_active.png)

## Where to find your subscriptions

1. From the main page of the website, click on the "My Account" button in the left bar ![My Account](images/main_page.png)
2. The new menu will open ![My Account page](images/My_account.png)
3. Click on the "SUBSCRIPTIONS" section. ![My Account page](images/My_account_sub_sec.png)
4. You can see all your subscriptions. ![Subscriptions](images/My_subs.png)

## How to connect to your virtual machine

You have several options to connect to your virtual machine:

- You can use the clients or applications for ssh connection. For example, PuTTY for Windows, or MobaXterm for Windows, Linux and Mac. You can download them from the internet. But for this option you need to configure the "SSH KEY" during creating virtual vachine (see [How to configure and setup SSH public keys, the right way](https://dev.to/gvelrajan/how-to-configure-and-setup-ssh-public-keys-the-right-way-23be)).
- You can use the connect to your virtual machine from the browser (see [How to connect to your virtual machine from the browser](#how-to-connect-to-your-virtual-machine-from-the-browser) section).
- Connect to your virtual machine using its IP by another software (see [How to see the IP of the virtual machine](#how-to-see-the-ip-of-the-virtual-machine) section).

## How to see the IP of the virtual machine

1. On the page of your virtual machine dashboard on the right side you can see the IP of your virtual machine ![IP](images/Your_Virtual_machine_dashboard_IP.png)
2. The IP looks like this: 10.13.127.89 ![IP](images/IP_mini.jpg)
3. If there is no IP - see [How to create a virtual machine with an explicit IP](#how-to-create-a-virtual-machine-with-an-explicit-ip-will-be-updated-soon) section.

## How to create a virtual machine with an explicit IP (will be updated soon)

1. Create a Network
2. Create a Virtual Machine with the Network you created

## How to connect to your virtual machine from the browser

1. From the page of your virtual machine dashboard, click on the "CONNECT" button on the bottom![Connect button](images/Vm_connect_button.png)
2. Then you can choose two options to connect to your virtual machine, to connect from the browser, click "WebConsole" ![Connect options web](images/Connect_choose_web.png)
3. The new browser window will open with your virtual machine console ![Web console](images/Vm_web_console.png)
4. You need to write your vm login (see [What is my virtual machine login](#what-is-my-virtual-machine-login)) and type enter
5. And then you need to write your vm password and type enter
6. If you see the message like "Login is incorrect" [Incorrect login or password](images/Login_is_incorrect.png). It means that you wrote incorrect login or password. Try again with correct login and password.
7. If you succesfully connected to your virtual machine, you can see the message "Welcome to Ubuntu 20.04.3 LTS (GNU/Linux 5.4.0-80-generic x86_64)" or something else depending on your virtual machine operating system ![Welcome message](images/Succesfull_login.png)
8. Now you can use your virtual machine as you want.

## How to see details of the created virtual machine

1. From the main page of the website, click on the "VIRTUAL MACHINES" button in the left bar ![Main virtual Machines](images/Main_virtual_machines.png)
2. Choose the virtual machine you want to see the details of and click on its name ![Virtual Machine details](images/Vm_details.png)
3. Then you can see the page with your virtual machine ![Your virtual machine details](images/Your_Virtual_machine_details.png)
4. If you want to see details, click "DASHBOARD" button ![Virtual Machine Dashboard button](images/Your_Virtual_machine_dashboard_button.png)
5. Then you can see the page with your virtual machine dashboard ![Your virtual machine dashboard one](images/Dashboard_1.png) ![Your virtual machine dashboard two](images/Dashboard_2.png)

## What is my virtual machine login

- At first, you can't see the login of your virtual machine when you have already created it. But more likely it is "root", "admin", or "administrator"
- You can see the login of your virtual machine during vm creation.
- For "QUICK START" option, you can see the login in the "ADMINISTRATOR ACCOUNT" section ![Quick start login](images/Quick_start_modal_login.png). The login is most likely lower-case instead of upper-case. Or you are required to fulfill it ![Fill the admin account](images/Quick_start_admin_account.png).
- For "FROM GALLERY" option, you can see the login in the "ADMINISTRATOR ACCOUNT" section ![From gallery login](images/Gallery_administrator_account_marked.png). The login is most likely lower-case instead of upper-case. Or you are required to fulfill it ![Fill the admin account](images/Gallery_administrator_account_marked.png).

## Password requirements

The password must contain 3 of the following:

- a lowercase character
- an uppercase character
- a number
- a special character

Example: MyP@ssw0rd123!

## Troubleshooting

If your screen became gray and you can't click anything, on the bottom you can see a message "Your session timed out. Cllick OK to log again". Don't worry, click "OK". You either need to log in again or just be redirected to main page.

Subscription is syncing too long: If your subscription is syncing too long - don't worry, more likely it is active right now and you can use it. If it is not, contact IT department of Innopolis University.

Virtual machine is creating too long: If your virtual machine is creating too long, try to delete and create virtual machine again. If you tried to do it several times, contact IT department of Innopolis University.

Virtual machine is failed to create: If you got such a message during creating a vm ![Failed to create message](images/Failed_to_create_message.png) you can see the details by clicking "i" button. Try to recreate virtual machine. If you tried to do it several times, contact IT department of Innopolis University.

If you have forgoten your password: contact IT department of Innopolis University.

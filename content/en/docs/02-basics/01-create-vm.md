---
title: "Create Virtual Machine"
weight: 30
---

## How to create a new virtual machine

1. At first, you need to have a subscription to the service (see [Subscriptions](../../01-setup/02-subscription/)).
2. From the main page of the website, click on the **VIRTUAL MACHINES** button in the left bar.
   ![Main Virtual Machines](../../../en/images/Main_virtual_machines.png)
3. On the Virtual Machines page, click on the **right arrow** button OR if you have already created some virtual machines, click on the **New** button in the left bottom corner and then **STANDALONE VIRTUAL MACHINE**.
   ![New VM](../../../en/images/Virtual_machines_empty_new.png)
4. In the opened menu you can choose a template for creating a virtual machine: quick start or from gallery.
   ![Choose Template](../../../en/images/VM_choose_template.png)

## How to create a new virtual machine from quick start

1. Menu with quick start creating will open.
   ![Quick Start Form](../../../en/images/Quick_start_form.png)
2. Here you need to write the name of your virtual machine into **NAME** field. Name is required.
3. Also choose the subscription type - depending on it you can choose different templates (operating systems) for virtual machine.
   ![Choose Subscription](../../../en/images/Choose_subscription_quick.png)
4. Then choose the template (operating system) for your virtual machine.
   ![VM Template](../../../en/images/Template_quick_start.png)
5. Write and confirm the new password for your virtual machine.
6. If you see the red exclamation mark in the **PASSWORD** field then the condition on the password is not satisfied (see [Password requirements](../../05-reference/01-password-policy/)).
7. "**ADMINISTRATOR ACCOUNT**" may be filled by default and can't be changed. But in some cases you are required to write your own name inside the field.
   ![Admin Account](../../../en/images/Quick_start_admin_account.png)
8. Save your password, administrator account and ssh key or product key, because you will not be able to see them again.
9. If all fields are filled correctly - click the **CREATE VM INSTANCE** button.
   ![Create VM Instance](../../../en/images/Create_VM_instance.png)
10. To see the details of creation - click on the **DETAILS** button.
    ![VM Details](../../../en/images/Started_creating_vm_details.png)
11. You can see the progress of creation of your virtual machine here.
    ![Creation Progress](../../../en/images/Creation_details_status.png)
12. On the Virtual Machines page you can see your virtual machine. For some time its status will be "Creating", then it will change to "Running".
    ![VM Running](../../../en/images/Vm_running.png)
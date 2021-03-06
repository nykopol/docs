---
title: Getting started with a VPS
excerpt: Learn the basics of using a VPS
slug: getting-started-vps
section: Getting started
order: 1
---

**Last updated 2018/04/18**
 
## Objective

A virtual private server (VPS) is a virtualized dedicated server. Unlike a web hosting service (called “shared”) where all technical management is done by OVH, you are fully responsible for the administration of your VPS.

**This guide will give you a few tips to help you manage your newly delivered and installed VPS.**


> [!warning]
>
> OVH is providing you with machines that you will be responsible for. We have no access to these machines, and therefore cannot manage them. You are responsible for day-to-day software and security management. This guide is designed to assist you in common tasks as much as possible. However, we recommend that you call upon a specialized service provider if you experience any issues or doubts when it comes to managing, using or securing your server. You can find more information in the “Go further” section of this guide.
> 


## Requirements

- You must have reserved your VPS on the [OVH website](https://www.ovh.com/ca/en/vps/){.external}.
- You must have received the email with your access ID after the installation (validated during the order).


## Instructions

Once you have logged in to your  [customer control panel](https://ca.ovh.com/auth/){.external}, to read the information about your VPS, simply go to the `Cloud`{.action} section, then to `Servers`{.action} in the left-hand column. In this section, you will see everything about your VPS: general information in the middle, operations you can perform listed as buttons on the right-hand side of the screen, and options at the very bottom.

### Logging in to a VPS

When you install (or reinstall) your VPS, an email will be sent to you with a password for root access, the login that uses the SSH protocol. SSH is a secure communication protocol. You can access the VPS through a command terminal (Linux or MAC) or through third-party software on Windows (e.g.: Putty).

Once you have opened the terminal, type the following command to log in to your VPS:

```sh
ssh root@IPv4_of_your_VPS
```

Or:

```sh
ssh root@your_VPS_reference_name
```

The reference name of your VPS always starts with vpsXXXX.ovh.net (where XXXX is a series of numbers).


### Installing or reinstalling your VPS

Any reinstallations can be carried out directly in your customer control panel. You simply need to click `Reinstall my VPS`{.action}:

![Reinstalling the VPS](images/reinstall_manager.png){.thumbnail}

A window will open, and you will need to choose:

- Your operating system in the proposed list
- The language
- An SSH key, if you have already created keys in your customer control panel.


![Reinstallation menu](images/reinstall_menu.png){.thumbnail}

> [!primary]
>
> Some operating systems or platforms such as Plesk or Windows require the purchase of a license prior to installation, which you can get either from OVH or from a reseller. You will then need to integrate it manually, or through your customer control panel. You can manage your licenses under `Dedicated`{.action}, then `Licenses`{.action}.
In this section, you can also order licenses (via the `Order`{.action} button on the right) or add your own SPLA Windows or SPLA SQL server license (`Add an SPLA license`{.action} button on the right).
> 

A progress bar will appear in your customer control panel, for the reinstallation - please note that it can take up to 30 minutes.


### Securing your VPS

As explained in the “Objective” section of this guide, you are the administrator of your VPS. As such, you are responsible for your data and its security.

Please refer to the guide on [Securing a VPS](https://docs.ovh.com/ca/en/vps/tips-for-securing-a-vps/){.external} if you wish to get some basic knowledge.


### Securing a domain with an SSL certificate

Once your VPS is installed and secured, you may want to secure your domain name and your website. To do this, you will need to install an SSL certificate, which will allow you to display your website in *https* rather than *http* only.

You can install this SSL certificate yourself manually, directly on the VPS. Please refer to the official documentation that you have been using.

For a more automated process, OVH also offers the [SSL Gateway](https://www.ovh.com/ca/en/ssl-gateway/). Please refer to the [product page](https://www.ovh.com/ca/en/ssl-gateway/){.external} on this solution.

## Go further

Join our community of users at <https://community.ovh.com/en/>.
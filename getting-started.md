---
copyright:
  years: 1994, 2017, 2018
lastupdated: "2018-03-16"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Getting started with Virtual Private Networking (VPN)

## What is IBM Cloud VPN?

VPN access enables users to manage all servers remotely and securely over the IBM Cloud private network. A VPN connection from your location to the private network allows out-of-band management and server rescue through an encrypted VPN tunnel. With VPN access, you can:

* Establish a VPN connection to the private network by SSL, PPTP, or IPSec.
* Access your server through its private 10.x.x.x IP address by SSH or RDP.
* Connect to your server’s IPMI IP address for additional server management or rescue needs.

**Note: PPTP VPN services will be deprecated effective June 12, 2018, as described in [our recent anouncement](pptp-deprecation.html).**

A number of services require access through the private network, and the VPN is one method that allows private network access. A VPN is good to use when you need to log in to the private network, do your work, and then log out. For example, this access often is needed to reach the KVM of the server.

Each user account can be given VPN access and can be limited regarding the subnets to which it needs access. You must have VPN access enabled and you must create a VPN password before you can log in to the VPN.

## Enable each user's VPN access

To get started, you'll need to enable VPN access on each account that needs VPN access. Every account starts with VPN access **disabled**, including your team's master account. To enable VPN access, follow these steps:

1. Go to **Account -> VPN Access** in the [Customer Portal ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://control.softlayer.com/).
* There you'll find the row for each possible VPN user and a link under the **VPN Access** column.
* The link will read "None" if the user does not yet have VPN access enabled.
* If the user's VPN access link reads **SSL, PPTP, or SSL & PPTP** that means that the user already has had their VPN access enabled.

![Softlayer Portal VPN Access table](images/vpnaccess01.png)

1. To enable or change the VPN access types permitted for a specific user, click the link under the **VPN Access** column.
* In the next page you can enable the VPN access type appropriate for each user.  
* By default, only one user can have PPTP VPN access. Should your account require more than one PPTP VPN user, please contact our Support Team via Live Chat, the Ticket System or by phone to enable unlimited PPTP VPN users at no cost.

![Assign VPN type access to a user](images/vpntype01.png)

## Set the VPN password

Your next step is to create a VPN password. Each user can create and update their VPN password in the [Customer Portal ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://control.softlayer.com/). To do so, select your name at the top right, which takes you to the **Edit profile** page. You can also select **Account -> Users** and then select your user name.

      Note: The link reads "Master User". This link will read your name for sub users.

On the **Edit User Profile** page, just scroll down and initialize or update the VPN password.

![ Edit Profile VPN password fields](images/vpnpasswordfields.png)

## Log in to the VPN

Now that the VPN access has been established, you can log in.

1. From IE you can log into the SSL VPN, visit [vpn.softlayer.com](https://vpn.softlayer.com/) and select any of the login points. You can use any VPN access point, and you are given the same access permissions to the private network in all the datacenters.
* If you have trouble logging into one location, try another location.
* Alternatively, you can log in using a standalone client SSL VPN. 
* You'll be able to use the standard OS utilities to log in to the PPTP VPN.

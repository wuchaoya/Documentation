
---
title: Release Notes
description: 
platform: iOS
updatedAt: Tue Feb 19 2019 07:16:08 GMT+0800 (CST)
---
# Release Notes
## Overview

The Agora Signaling SDK facilitates real-time communications through functions such as call invitations, messaging, and state synchronization.

### Known Issues and Limitations

-   Each channel can hold up to 10,000 users at the same time. To reduce data volume and stress on the SDK, Agora recommends disabling notifications of a user going online or dropping offline for a large channel holding more than 1,000 users. For more information, see the `channelSetAttr` method. 
-   Channel Messages:
    -   Each message can be up to 8-K visible characters.
    -   A user can send messages at a maximum speed of 60 messages per second. In a channel, a maximum of 200 messages can be sent each second. Messages exceeding this limit will be discarded. 
    -   Offline channel messages are not supported.
    -   Supports the string type and UTF-8 character encoding only.
-   Point-to-point messages:
    -   Each message can be up to 8-K visible characters.
    -   Offline messages are not supported.
    -   Supports the string type and UTF-8 character encoding only.
-   Channel-attributes-updated callback:
    -   A maximum of 10 channel-attributes-updated callbacks can be sent each second.

## v1.4.4

The version 1.4.4 was released on December 13, 2018. See below for issues fixed.

- Fixed a couple of crash issues on iOS. 
- Improved the code implementation for iOS. 

## v1.4.0 

The version 1.4.0 was released on August 24, 2018. See below for new features and issues fixed.

-   Added support for creating multiple signaling instances.
-   Fixed a crash issue caused by the DNS.


## v1.3.3 

The version 1.3.3 was released on July 11, 2018. See below for issues fixed.

Fixed a crash issue caused by the DNS.

## v1.3.0 

The version 1.3.0 was released on May 4, 2018. See below for new features.

-   Added support for bitcode.
-   Added a special <code>_timeout</code> attribute to the <code>extra</code> parameter of <code>channelInviteUser2</code> to set the call timeout equal to or greater than 1 s.
-   Added support for the CocoaPods package management tool, `AgoraSig\iOS-1.3.0.zip`.


## v1.2.1

The version 1.2.1 was released on March 20, 2018. See below for issues fixed.

Fixed the following issues:

-   Memory leakage.
-   Triggering of some callbacks.


## v1.2.0

The version 1.2.0 was released on March 7, 2018. See below for new features.

-   Added the <code>invoke</code> calling mechanism.
-   Added internal channel attributes, including `_channel_ttl`, `_member_num`, and `_auto_update_num`.
-   If you are currently logged in, any call of the <code>login</code> method will be neglected.
-   To abandon the previous login, you only need to call <code>logout</code> before calling <code>login</code> without having to wait until it is successfully executed.


## v1.1.4.19

The version 1.1.4.19 was released on November 4, 2017. See below for issues fixed.

Fixed IPv6 related issues.

## v1.1.3 

The version 1.1.3 was released on August 16, 2017. See below for improvements.

Improved the quality and stability of the signaling system login.

## v1.1.1

The version 1.1.1 was released on March 10, 2017.

Internal improvements.

## v1.0

The version 1.0 was released on September 30, 2016.

This is the first release of the Agora Signaling SDK, which includes:

-   The Agora Signaling SDK for Android
-   The Agora Signaling SDK for iOS
-   The Agora Signaling SDK for Windows
-   The Agora Signaling SDK for Mac


The Agora Signaling SDK provides the following functions:

-   Account Information System
-   Channel System
-   Call System


You can access the Agora Signaling System in the following ways:

-   SDK Access
-   Server API Access
-   SIP Gateway Access





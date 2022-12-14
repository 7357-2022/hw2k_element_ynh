<!--
N.B.: This README was automatically generated by https://github.com/YunoHost/apps/tree/master/tools/README-generator
It shall NOT be edited by hand.
-->

# Element for YunoHost (forked for the HW2K website)

[![Integration level](https://dash.yunohost.org/integration/element.svg)](https://dash.yunohost.org/appci/app/element) ![Working status](https://ci-apps.yunohost.org/ci/badges/element.status.svg) ![Maintenance status](https://ci-apps.yunohost.org/ci/badges/element.maintain.svg)  
[![Install Element with YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=element)


> *This package allows you to install Element quickly and simply on a YunoHost server.
If you don't have YunoHost, please consult [the guide](https://yunohost.org/#/install) to learn how to install it.*

## Overview

Element is a new type of messaging app. You choose where your messages are stored, putting you in control of your data. It gives you access to the Matrix open network, so you can talk to anyone. Element provides a new level of security, adding cross-signed device verification to default end-to-end encryption.

**Shipped version:** 1.11.17~ynh1

**Demo:** https://app.element.io/

## Screenshots

![Screenshot of Element](./doc/screenshots/homepage-all-platforms-1_1.png)

## Disclaimers / important information

## YunoHost specific features

### Multi-users support

This application support the SSO. If you want to use the SSO, you need to define the path to the default homeserver as your homeserver witch is installed on your YunoHost instance.

## Additional informations

### Important Security Note

We do not recommend running Element from the same domain name as your Matrix
homeserver (Synapse).  The reason is the risk of XSS (cross-site-scripting)
vulnerabilities that could occur if someone caused Element to load and render
malicious user generated content from a Matrix API which then had trusted
access to Element (or other apps) due to sharing the same domain.

We have put some coarse mitigations into place to try to protect against this
situation, but it's still not good practice to do it in the first place.  See
https://github.com/vector-im/riot-web/issues/1977 for more details.

## Documentation and resources

* YunoHost app: https://github.com/YunoHost-Apps/element_ynh
* Official app website: <https://element.io>
* Official admin documentation: <https://element.io/help>
* Upstream app code repository: <https://github.com/vector-im/element-web/>
* YunoHost documentation for this app: <https://yunohost.org/app_element>
* Report a bug: <https://github.com/YunoHost-Apps/element_ynh/issues>

## Developer info

Please send your pull request to the [testing branch](https://github.com/7357-2022/hw2k_element_ynh/tree/testing).

To try the testing branch, please proceed like that.

``` bash
sudo yunohost app install https://github.com/7357-2022/hw2k_element_ynh/tree/testing --debug
```
or
```
sudo yunohost app upgrade element -u https://github.com/7357-2022/hw2k_element_ynh/tree/testing --debug
```

**More info regarding app packaging:** <https://yunohost.org/packaging_apps>

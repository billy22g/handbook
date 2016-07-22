---
title: Ubuntu
---

Ubuntu is a Debian-based Linux operating system.

## Setup

See [Eric's Macbook Pro installation instructions](https://github.com/konklone/ubuntu/blob/master/macbook.md) for Macbook Pro model `11,2` (you likely have this).

## Downsides and bugs

There are known problems with Ubuntu:

- **The webcam doesn't work yet.** In 2013, Apple switched the iSight camera from USB to PCI Express, and there isn't a Linux driver for it yet. Subscribe to [this bug](https://bugs.launchpad.net/ubuntu/+source/linux/+bug/1276811) to watch the issue.
- **Thunderbolt displays don't work.** Other external monitors should work fine.

## Connecting to Wi-Fi

See our [networks](https://handbook.18f.gov/networks/) guide for general tips.

1. Click the **Wireless** menu in your system tray and select **Connect to Hidden Wi-Fi Network...**
2. Under **Network name**, enter `gsa-wireless`.
3. Under **Wi-Fi security**, choose **WPA & WPA2 Enterprise**.
4. Under **Authentication**, choose **Protected EAP (PEAP)**. Leave **Anonymous identity** alone.
5. Check the **No CA certificate is required** checkbox. Leave **CA certificate** blank. Leave **PEAP version** and **Inner authentication** alone.
6. Under **Username** and **Password**, enter `ENT/YourName`, replacing `YourName` with your ENT username and password. Note the _forward_ slash, `/` -- not the backslash you may have seen when logging into your Dell.
7. Try to connect.
8. If it fails, edit `/etc/NetworkManager/system-connections/gsa-wireless` and look for a line that says `system-ca-certs=true`. Delete it, or change it to say `system-ca-certs=false`. Then try again. See [Fixing WPA2 Enterprise in Ubuntu](http://askubuntu.com/a/292072) if you're still having trouble.

## Connect to a printer

1. Download the [generic driver for the Xerox ColorQube 9303](http://www.support.xerox.com/support/colorqube-9300-series/file-download/enus.html?operatingSystem=winxp&fileLanguage=en&contentId=116360&from=downloads&viewArchived=false). Inside the zip file, you will need `XeroxColorQube9303.ppd`.
2. Open the Printers management area. Click **Add**, and on the New Printer dialogue that comes up, toggle **Network Printer** and click **Find Network Printer**.
3. Enter the IP address of the 18F printer in your [office guide](https://handbook.18f.gov/offices), and click **Find**.
4. It should bring up a port and connection -- the defaults are fine, click **Forward**.
5. It'll search unsuccessfully for a driver online. When it asks you for the driver, choose **Provide PPD file** and select `XeroxColorQube9303.ppd` from disk.
5. **You're not done!** By default, the printer is configured to print to Tray 1, which is wrong. Under the properties for the printer you added, open **Printer Options**, and change the paper tray to Tray 3.
6. Print a test page, and should it print, rejoice.

![Successful test print page]({{ site.baseurl }}/images/ubuntu/ubuntu-printer.jpg)

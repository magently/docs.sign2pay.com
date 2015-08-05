---
layout: default
title: Magento integration
---

<ol class="breadcrumb">
  <li><a href="/">Home</a></li>
  <li><a href="/integrations/index.html">Integrations</a></li>
  <li>Magento</li>
</ol>

# Integrating Sign2Pay with Magento

Sign2Pay has native integration with Magento. This guide will show you how to upload and configure our official extension.

## Create an Application

The first step is to register your merchant account with us. Our general setup guide has you covered. Please go ahead and follow that, we’ll wait here when you get back. ;-) [Go to general setup now.](http://docs.sign2pay.com/merchant-admin/)

## Download Module

After you’ve created your merchant application with us, choose the native Magento integration. In your Sign2Pay admin homepage choose “Manage Application” and then select Magento as the implementation type.

<img src="../../images/integrations/magento/Schermafbeelding_2014-12-02_om_14_30_36-1024x899.png">

You can then download the module on the right hand side of the screen.

<img src="../../images/integrations/magento/Schermafbeelding_2014-12-02_om_14_30_361-1024x899.png">

You can also download the extension directly: [https://github.com/Sign2Pay/magento-sign2pay/releases](https://github.com/Sign2Pay/magento-sign2pay/releases). This shows you a list of versions, with the most recent version at the top. Download either the .zip or .tar.gz archive and upload this to your Magento admin.

## Installation

Installation of our extension works like any other Magento extension. In the Magento Admin, choose System > Magento Connect > Magento Connect Manager:

<img src="../../images/integrations/magento/Schermafbeelding_2014-12-03_om_10_33_51-1024x899.png">

After entering your admin password again, look for the heading “Direct package file upload”. At step 2 (Upload Package File) choose the extension file you’ve downloaded from our website and click Upload.

<img src="../../images/integrations/magento/Schermafbeelding_2014-12-03_om_10_39_11-1024x899.png">

This will install the extension. You should see the process at the bottom of the screen. When it’s installed, you can return to the Magento Admin.

## Configuration

Choose System > Configuration.

In the menu on the left, choose *Payment Methods*. Sign2Pay will be listed as one of the payment methods. Click on the heading Sign2Pay. You should see this screen:

<img src="../../images/integrations/magento/Schermafbeelding-2014-12-03-om-10.43.19-1024x899.png">

In the fields for Merchant ID, Application Token and API Token fill in the values you find in your Application Settings in the [Sign2Pay Merchant Admin](https://merchant.sign2pay.com/).

Settings overview:
<dl>
	<dt>Enable Sign2Pay</dt>
	<dd>Selecting "Yes" enables Sign2Pay on checkout screen.</dd>
	<dt>Complete Order Status</dt>
	<dd>The order status right after the payment capture.</dd>
	<dt>New Order Status</dt>
	<dd>The order status after order placement.</dd>
	<dt>Merchant ID</dt>
	<dd>The Sign2Pay merchant identifier.</dd>
	<dt>Application Token</dt>
	<dd>The Sign2Pay application token.</dd>
	<dt>API Token</dt>
	<dd>The Sign2Pay api token.</dd>
</dl>

When you are done, click *Save Config* at the top of the screen.

## Compatibility and requirments

Following Magento versions were successfully tested:
<ul>
	<li>
		Community Edition
		<ul>
			<li>1.9</li>
			<li>1.8</li>
			<li>1.7</li>
		</ul>
	</li>
	<li>
		Enterprise Edition
		<ul>
			<li>1.14</li>	
		</ul>
	</li>
</ul>

Following Magento checkout extensions were successfully tested:
<ul>
	<li>(IWD) <a target="_blank" href="http://www.magentocommerce.com/magento-connect/one-page-checkout.html">One Page Checkout</a></li>
	<li>(Magestore) <a target="_blank" href="http://www.magentocommerce.com/magento-connect/one-step-checkout-7-4908.html">One Step Checkout</a></li>
</ul>
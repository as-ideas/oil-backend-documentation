# Introduction
## About OIL - Backoffice
The OIL Backoffice Service is a stable cross-company solution that provides for easy configuration and integration of [OIL.js](https://github.com/as-ideas/oil) in any website.
It is a web application with the following feature set:

* OIL.js Configuration Manager

  You can create and persist your own configuration for OIL.js. Every change creates a new configuration version stored in a version history that allows to (re-)view any older version.
  
* OIL.js Localizing Manager

  You can create and persist your own localizings for OIL.js labels - the locales. Every change creates a new locale version stored in a version history that allows to (re-)view
  any older version. Locales are defined globally and can be (re-)used by all clients of the OIL Backoffice Service by integrating them in their OIL.js configuration.
  
* Client-specific OIL.js package provided through a Content Delivery Network (Amazon CloudFront)

  You can create your very own OIL.js package containing your specific configuration and localizing. You can upload it to our Content Delivery Network (Amazon CloudFront) and 
  integrate it in your website with only two simple 'script' tags.

## Account
To access the OIL Backoffice Service an account is required. To get one please send an email to [oil-support@asideas.de](mailto:oil-support@asideas.de). As soon as you are entitled
to access the OIL Backoffice Service

1. Go to [https://oil-backend.herokuapp.com/oil/](https://oil-backend.herokuapp.com/oil/) and
2. Sign in to the web application

## Pages Overview
### My Configurations

This page provides an overview of your configuration versions. Click the "Update Configuration" button to view an existing version that you can update now (see section 
[Configuration Manager](#configuration-manager) for details). If you don't have an older configuration version you can create a new one by clicking the "(+) Add New" button.

![OIL-JS Configuration](documentation/my-configuration.jpg?raw=true)

The newest version is always marked as "Currently used configuration". To activate it and to create your very own OIL.js package containing it please

1. Choose the OIL.js version using the drop-down box in the upper right corner. We recommend to always use the latest version. Please check the OIL.js release notes and
documentation for the feature set of previous OIL.js releases.
2. Click the "Upload Package" button. This will create your OIL.js package and upload it to our Content Delivery Network (Amazon CloudFront). After that an HTML code snippet is
shown that you should use to integrate this OIL.js package in your website. Please do not change it, otherwise the integration will not work.

### Configuration Manager
This is the detailed configuration manager for OIL.js showing all parameters of your (selected) OIL.js configuration version. To enables you to update your configuration all
parameters are changeable. Updating means you can make any changes you want and save them by clicking the "Save new version" button. This will create a new version. The original
version stays always unchanged. The configuration manager provides a simple validation for the parameter values. For all parameters a short help text is offered. Click on the
information icon (i) to show it.

![OIL-JS Configuration](documentation/oil-confuguration-manager.jpg?raw=true)

Note: If you want to use another locale than the default, you have to go to the "Locale" tab. Here you can select one of the existing locale versions. See the [Localization](#localization) section
for details how to define a new locale version.

To get an overview of OIL.js configuration parameters please read the [OIL-Documentation](https://oil.axelspringer.com/docs/last-release) (Section "Functional Configuration Parameters").

### Custom Vendors
This page provides an overview of your Custom Vendors.

You can add new Custom Vendor or edit existing Custom Vendors.



### Custom Vendors Lists

### Localization

This page provides an overview of all locales that are currently available. A locale is defined by its name (locale id) and version. You can choose an existing locale using the
two drop down elements "Locale Id" and "Version" or you can add new one by clicking the "(+) Add New" button. Please note that an existing locale version cannot be changed. As
for configurations only creation of a new version is possible.

![OIL-JS Configuration](documentation/new-locale.jpg?raw=true)
![OIL-JS Configuration](documentation/locale-configuration.jpg?raw=true)

To get an overview of OIL.js locales and their labels please read the [OIL-Documentation](https://oil.axelspringer.com/docs/last-release) (Section "Language label configuration").

## Complete round trip or How to integrate OIL.js in your website?

Please follow these steps:

1. Get an account OIL Backoffice Service.
2. Go to [https://oil-backend.herokuapp.com/oil/](https://oil-backend.herokuapp.com/oil/) and sign in.
3. Check existing locales. If none of them suits your needs create a new one.
4. Add a new OIL.js configuration.
5. Select your OIL.js version and click on the "Upload Package" button.
6. Integrate the shown HTML code snippet into your website (within the HEAD section).

Congratulations! You're done.


 

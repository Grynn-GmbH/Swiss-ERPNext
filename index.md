# erpnextswiss 

**erpnextswiss** is a customization of [erpnext](https://erpnext.com/) for switzerland opensourced by [grynn](https://grynn.ch). It Contains Features That Makes [erpnext](https://erpnext.com/) Usable for Switzerland Market. Customizations are Created With flexibility in Mind so you can Pick any of the Customization without Worrying About Other. Eg. You can only Install out app that Creates QRBILL without installing the whole suite. Customizations are as follows

1. [ Swiss-E-invoicing-ERPNext](https://github.com/Grynn-GmbH/Swiss-E-invoicing-ERPNext) : Swiss E Invoicing PDF For ERPNEXT by Grynn
2. [Swiss-QR-Bill-ERPNext](https://github.com/Grynn-GmbH/Swiss-QR-Bill-ERPNext) : Swiss QR Bill by Grynn
3. [ESTV-SuisseTax-FX](https://github.com/Grynn-GmbH/ESTV-SuisseTax-FX) : ERPNext for Switzerland By Grynn - Automated Daily & Monthly Import of FX Rates



## Swiss-E-invoicing-ERPNext

Swiss-E-Invoicing-ERPNext is a App/Plugin for creating E-invoicing as you create sales invoice. with this app/plugin you can automatically create **E-Invoice PDF** and attach it to your **Sales Invoice**. It creates a machine readable XML as per standard FACTUR-X and creates a standard bill as per your default sales invoice template and then creates the attachment.

### Installation (Frappe Cloud) 

....

### Installation (For Developers)

```sh
$ cd <your-bench-directory>
$ bench get-app grynnswissqrbill https://github.com/Grynn-GmbH/Swiss-E-invoicing-ERPNext
$ bench --site <your-site> install-app grynnswissqrbill
$ bench restart
```



### Prerequisite / Settings

There are no Prerequisite to this application but it is good to have following settings.

1. Company Generating Sales Invoice have Address Assigned to it.

##### For Assigning Address to Company 

![Add Company](./assets/add-company.gif)

## usage

Using Swiss-E-Invoice-ERPnext is fully automated, you just need to create a Sales Invoice and It Generates the PDF and Attaches it to Sales Invoice



##  Swiss QR Bill for ERPNext

![Swiss QR Bill Types](./assets/qrtypes.jpg)Grynn has developed a QR Bill Generator app (Free and Open Source) that works seemlessly with ERPNext. The Swiss QR Bill can be used in 3 different ways. We have implemented the general version for IBAN, without Reference. 

### Installation (Frappe Cloud) 

....

### Installation (For Developers)

```sh
$ cd <your-bench-directory>
$ bench get-app grynnswissqrbill https://github.com/Grynn-GmbH/Swiss-E-invoicing-ERPNext
$ bench --site <your-site> install-app grynnswissqrbill
$ bench restart
```

### Prerequisite / Settings

There are Mandatory Prerequisite for the application as follows

1. Company Country Should Be Grynn
2. Currency of Sales Invoice Should be Either `CHF` or `EUR`
3. Sales Invoice Customer Address Should be From Switzerland

### Usage

Using Swiss-QR-Bill-ERPNext is fully automated, you just need to create a Sales Invoice and It Generates the PDF and Attaches it to Sales Invoice



## ESTV-SuisseTax-FX

ESTV-SuisseTax-FX is a cron/scheduled application which daily updates your exchange rate with other currencies. It uses Exchange Rate Provided [Here](https://www.backend-rates.ezv.admin.ch/api/xmlavgmonth) to Fetch daily and monthly exchange rates. 

### Installation (Frappe Cloud) 

....

### Installation (For Developers)

```sh
$ cd <your-bench-directory>
$ bench get-app estv_suissetax_fx https://github.com/Grynn-GmbH/Swiss-E-invoicing-ERPNext
$ bench --site <your-site> install-app estv_suissetax_fx
$ bench restart
```



### Prerequisite / Settings

in order to enable entries for fx rates for a particular currency you need to enable it through currencies.

![Enable Currency](./assets/currency.gif)



### Usage

Using ESTV-SuisseTax-FX is fully automated, you just need to create a Sales Invoice and It Generates the PDF and Attaches it to Sales Invoice



## Check Installed Applications

#### Step 1: 

Click on ERPNext Logo and Go to your Homepage of Desk

![](./assets/step-1-installation.png)

#### Step 2:

![](./assets/step-1-help.png)

#### Step 3: 

Click On About

![](./assets/step-2-about.png)

#### Step - 4 

In about section it should show the installed apps with their versions. Like Here Estv Suissetax FX, Grynnswissqrbill & Swiss Factur X E Invoicing is installed in our site

![](./assets/step-4.png)



## License

Every App/Plugin are provided under [GPLV3](https://en.wikipedia.org/wiki/GNU_General_Public_License) License and swisserpnext is developed and maintained by  [Grynn](https://grynn.ch)



## Requirements

To use these customizations you need [erpnext](https://github.com/frappe/erpnext) & That is the only requirement.



## Privacy

All the App/Plugin Created for ERPNext by Grynn does not Take any of Your Data. Privacy is a key factor for grynn and every software provided for customization ensures privacy.



## Contributions

Contributions to any of our applications are welcome. 



## Issues

issues specific to app/plugin can be found as follows, these issues mean known bugs to a specific application. this medium is specifically used to file any malfunction of software

1. [ Swiss-E-invoicing-ERPNext Issues](https://github.com/Grynn-GmbH/Swiss-E-invoicing-ERPNext/issues) 
2. [Swiss-QR-Bill-ERPNext Issues](https://github.com/Grynn-GmbH/Swiss-QR-Bill-ERPNext/issues) 
3. [ESTV-SuisseTax-FX Issues](https://github.com/Grynn-GmbH/ESTV-SuisseTax-FX/issues) 



## Contact

If you would like us to implement the other two types, kindly get in touch with us. sales@grynn.ch. 



## Grynn's Mission : Promote & Implement ERPNext for Swiss Companies

Grynn GmbH loves, implements & promotes ERPNext in Switzerland, Germany, Eastern Europe and India. 

Founded in 2017 by Deepak Pai in order to help companies with their digital transformation journey. He has 2 decades of IT and Finance & has worked for companies such as Bank of America, Unilever and Ecolab. He is an MBA graduate of St. Gallen University (Switzerland) and alumnus of MIT Manipal. He is a certified digital strategist from MIT/Emeritus & consults for F500 companies.



## Grynn and Open Source

Grynn is an advocate of using Free and Open Source Software (FOSS). ERPNext is world's #1 ERP system that is 100% FOSS. 
Grynn from time to time contributes to the ERPNext ecosystem by developing Open Source applications such as Swiss QR Bill. 



### Logo and Trademark

The brand Grynn and the logo are trademarks for Grynn GmbH.
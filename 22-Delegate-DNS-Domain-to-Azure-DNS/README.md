# Title: Delegate DNS Domain to Azure DNS 

![](https://i.imgur.com/waxVImv.png)
### [View all Roadmaps](https://github.com/nholuongut/all-roadmaps) &nbsp;&middot;&nbsp; [Best Practices](https://github.com/nholuongut/all-roadmaps/blob/main/public/best-practices/) &nbsp;&middot;&nbsp; [Questions](https://www.linkedin.com/in/nholuong/)
<br/>

# Description: Learn to Delegate DNS Domain to Azure DNS 
## Important Note: DNS Domain
- This demo requires registered DNS Domain, if you don't have one just please go through the demo to know more about Azure Public DNS Zones

## Step-01: Introduction
- Understand about
  - Domain Registrar
  - DNS Zones
- Learn to delegate a domain from AWS Route53 to Azure DNS by creating DNS Zones in Azure Cloud 


## Step-02: DNS Zones - Create DNS Zone
- Go to Service -> **DNS Zones**
- **Subscription:** nholuongut-Paid-Subscription (You need to have a paid subscription for this)
- **Resource Group:** dns-zones
- **Name:** nholuongut.com
- **Resource Group Location:** East US
- Click on **Review + Create**

## Step-03: Make a note of Azure Nameservers
- Go to Services -> **DNS Zones** -> **nholuongut.com**
- Make a note of Nameservers
```
ns1-04.azure-dns.com.
ns2-04.azure-dns.net.
ns3-04.azure-dns.org.
ns4-04.azure-dns.info.
```

## Step-04: Update Nameservers at your Domain provider (Mine is AWS)
- **Verify before updation**
```
nslookup -type=SOA nholuongut.com
nslookup -type=NS nholuongut.com
```
- Go to AWS Route53 (This is my Domain Provider)
- Go to Services -> Route53 -> Registered Domains -> nholuongut.com
- Click on **Add or edit name servers**
- Update Azure Name servers here and click on **Update**
- Click on **Hosted Zones**
- Delete the hosted zone with name **nholuongut.com**
- **Verify after updation**
```
nslookup -type=SOA nholuongut.com 8.8.8.8
nslookup -type=NS nholuongut.com 8.8.8.8
```

![](https://i.imgur.com/waxVImv.png)
# 🚀 I'm are always open to your feedback.  Please contact as bellow information:
### [Contact Me]
* [Name: Nho Luong]
* [Skype](luongutnho_skype)
* [Github](https://github.com/nholuongut/)
* [Linkedin](https://www.linkedin.com/in/nholuong/)
* [Email Address](luongutnho@hotmail.com)
* [PayPal.me](https://www.paypal.com/paypalme/nholuongut)

![](https://i.imgur.com/waxVImv.png)
![](Donate.png)
[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/nholuong)

# License
* Nho Luong (c). All Rights Reserved.🌟
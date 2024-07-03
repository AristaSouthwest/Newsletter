 ![Image Placememt](img/Arista_Logo_copy.png)


# Arista May Southwest Region Newsletter

Welcome to the July 2024 newsletter for Arista customers in the U.S. Southwest Region!
 
We welcome your feedback on the newsletter. If you have any ideas on what you want to see, please reach out to southwest@arista.com.

---

## **Smart System Upgrade** 
By: Murthy Devarakonda, SE Manager Southwest Region

IT networks are increasingly becoming important to various organizations. Networks enable organizations to be agile in conducting business and improve overall performance. Networks are especially crucial in mission-critical environments like hospitals, where patient data and vitals are transferred through the network for better care. Network architects build networks to provide device and link-level redundancies to address unexpected failures. However, the network operations team, which manages the network, is always concerned about network device software upgrades and the possible downtime they can bring. 

Due to this concern, the majority of operations teams delay software upgrades. However, these delays can expose the network infrastructure to vulnerabilities and potentially allow malicious actors to breach the network. While most network vendors promise software upgrades with less downtime, only Arista has been able to provide near zero downtime upgrades. Even though software upgrades are typically performed during a maintenance window, reducing or eliminating downtime remains a key metric for most networks. 

In this article, I will discuss the Smart System Upgrade process, which reduces network downtime during software upgrades. A typical enterprise network consists of aggregation and leaf layer switches, as shown in the diagram below.

<figure markdown>
![Image Placement](img/Newsletter_July2024_pic1.png)
    <figcaption>Aggregation and Leaf Layer Switches </figcaption>
</figure>

In the above architecture, the aggregation layer switches can be upgraded one at a time to avoid network downtime at that layer using MLAG In-State Software Upgrade (MLAG ISSU) process. In this process, Arista EOS verifies the MLAG health before and after the upgrade to avoid network connectivity disruptions to both downstream and upstream network devices. Typically, endpoints at the leaf layer are single-homed. Arista's Smart System Upgrade (SSU) can reduce downtime to sub-second, and in most cases, the endpoints do not even notice the outage. In this upgrade process, Arista EOS will continue to forward the network traffic in the dataplane while upgrading the control plane. Once the control plane is upgraded to the latest version, it will reset the dataplane to achieve sub-second outage. The upgrade operation can be performed through CLI or through the CloudVision management platform. Upgrading the switch software through CloudVision provides additional controls like pre and post verifications through actions.

<figure markdown>
![Image Placement](img/Newsletter_July2024_pic11.png)
    <figcaption>High Availability Features </figcaption>
</figure>


Links for more information are below:  
[Hitless Upgrade - The Whats, The Whys, and The Hows](https://arista.my.site.com/AristaCommunity/s/article/Hitless-Upgrades-The-Whats-The-Whys-and-The-Hows)  
[Smart System Upgrade User Manuel](https://www.arista.com/en/um-eos/eos-smart-system-upgrade)  


---

## **Multi-Chassis Link Aggregation (MLAG)**
By: Alex Bojko, Advanced Services Engineer Southwest Region

MLAG is Arista's open standards based solution for achieving Active-Active forwarding at Layer 2 of the OSI model. In this article, I will explain the benefits and components that make MLAG possible.  

When designing the optimal network, redundancy, scalability, and high availability are top of mind. We want to eliminate single points of failure, plan for the future, and ensure that mission critical applications and services are always operational. When purchasing devices and cabling for the optimal network, we want to fully leverage the capacity and bandwidth of those devices and cables. For example, if you purchase a high end sports car, you wouldn't want a governor stopping you from achieving maximum speed and performance of your vehicle. In that same regard, we want our network to be able to leverage the available bandwidth and capacity to its maximum potential, all while achieving redundancy, scalability, and high availability.  

MLAG (Multi-chassis Link Aggregation) meets the demands of the optimal network while maximizing the bandwidth utilization and compute capacity of the available links and devices within our network. MLAG leverages open standards based LACP and expands on the functionality of standard port-channels. 

<figure markdown>
![Image Placement](img/Newsletter_July2024_article2.png)
    <figcaption>Configlet Table</figcaption>
</figure>


MLAG consists of two physical peer switches that logically appear as a single device by advertising the same shared mac-address to downstream devices while syncing mac-address tables between the two peers. MLAG is an enhancement to a standard LAG because it splits a LAG group across different nodes, allowing downstream devices to be dual-homed to the MLAG Domain. MLAG eliminates any STP blocked ports while facilitating active-active forwarding at L2. This allows for full bandwidth utilization of our physical links as well as full compute capacity since both peer devices are in an active forwarding mode, advertising the same shared mac-address. Also, when it comes time to upgrade the devices, MLAG In-State Software Upgrade (MLAG ISSU) allows us to upgrade one peer device at a time, eliminating any downtime windows while continuing to forward traffic as expected.  

By implementing MLAG, we receive link and device level redundancy, scalability with the capacity to support a large amount of downstream hosts, and high availability for our mission critical applications and services.


Links for additional information:  
[MLAG Configuration Guide](https://arista.my.site.com/AristaCommunity/s/article/mlag-basic-configuration)  
[MLAG Explanation](https://www.arista.com/en/products/multi-chassis-link-aggregation-mlag)  


---

## __*Upcoming Events*__  
Arista hosts various events throughout the year for you! Members of our team organize these informative events to showcase Arista's ability to not only help improve your network, but to also assist by providing a set of tools to improve your operations! Click on the boxes below to be directed to Arista's website for lists of Webinars and Events.


<div class="grid cards" markdown>

-   __Webinars__  

    --- 

    We make is easy for you to view products that are of interest, all virtually! Technical memebers of the team showcase outstading explanation of the products. Click below to see our list of Webinars. 

    [Arista Webinars](https://www.arista.com/en/company/news/webinars){.md-button}

-   __Events__ 

    ---
    Join us in person to get a closer look in our list of produts and solution, as well as get the chance to meet members of the team. Click below to see our list of ipcoming Events. 

    [Upcoming Events](https://www.arista.com/en/company/news/events){ .md-button }


</div>

--- 

## __*Software Updates*__
<figure markdown>
![Image Placement](img/pictureOfCloudVision.jpeg){: style="height:200px;width:300px"}    
    <figcaption></figcaption>
</figure>
For new code releases, click [here](https://www.arista.com/en/support/software-download) 


   |  Softwares    | Versions      |  Release Date |
   | :-----------: | :-----------: | :-----------:
   | __EOS__           | 4.32.0.1F <br>4.26.14M <br>4.29.8M<br>4.28.11M<br>4.31.3M<br>     | May 16th, 2024 <br>May 15th, 2024<br>May 14th, 2024<br>May 3rd, 2024<br>May 1st, 2024<br>
   | __CVP__           | 2023.3.2 <br>2024.1.2<br>     | May 14th, 2024 <br>May 10th, 2024<br>
   | __DMF__           | 8.5.0         | February 5th, 2024
   | __WLAN__ <br>CV-CUE<br>Wireless Manager<br> | <br>13.0.0-67<br>15.0.1-22<br>       | <br>December 15th, 2022<br>August 29th, 2023<br>
   | __Arista NDR__         | 5.1.2         | February 15th, 2024
   | __TerminAttr__    | 1.32.1        | June 13th, 2024


---

## __*Software Advisories*__
Below is a list of advisories that are announced by Arista. To view more details on the specific advisories, please click the links in the middle boxes.

| Name          | Advisory Link           | Date of Advisory Notice  |
| :-----------: |:-------------:| :-----:|
| __EOS with OpenConfig__   | [Security Advisory 0099](https://www.arista.com/en/support/advisories-notices/security-advisory/19862-security-advisory-0099) | July 2nd, 2024
| __Wireless Access Points__   | [Security Advisory 0098](https://www.arista.com/en/support/advisories-notices/security-advisory/19844-security-advisory-0098) | June 25th, 2024
|  __SSID Confusion__   | [Security Advisory 0097](https://www.arista.com/en/support/advisories-notices/security-advisory/19476-security-advisory-0097)  | May 24th, 2024   |
| __802.1x Authentication on Ports__    | [Security Advisory 0096](https://www.arista.com/en/support/advisories-notices/security-advisory/19462-security-advisory-0096) |   May 21st, 2024             |
| __XZ Tarballs__              |  [Security Advisory 0095](https://www.arista.com/en/support/advisories-notices/security-advisory/19222-security-advisory-0095)             | April 3rd, 2024       |
| __HTTP/2 Continuation Frames__    | [Security Advisory 0094](https://www.arista.com/en/support/advisories-notices/security-advisory/19221-security-advisory-0094)               | April 5th, 2024             |

For a list of the most current advisories and notices, click [Here](https://www.arista.com/en/support/advisories-notices)

---

## __*Product Updates*__
<figure markdown>
![Image Placement](img/pictureOfSwitches.jpeg){: style="height:200px;width:400px"}   
    <figcaption></figcaption>
</figure>
**End of Sale** notices are listed below.

| Device        | Name           | End Of Sale Date  |
| :-----------: |:-------------: |     :----:        |
| Module        | [7500R2 Series Linecards](https://www.arista.com/en/support/advisories-notices/end-of-sale/18886-end-of-sale-of-the-arista-7500r2-series-line-cards) | December 20th, 2023    |
| Access Points | [Arista 802.11ac Wave 2 Devices](https://www.arista.com/en/support/advisories-notices/end-of-sale/14911-end-of-sale-of-arista-802-11ac-wave-2-devices)      |  June 30th, 2022 |
| DMF           | [DMF/CCF Appliances](https://www.arista.com/en/support/advisories-notices/end-of-sale/19298-end-of-sale-end-of-life-for-arista-ccf-appliances-dca-dm-cdl-and-dca-cc-cdl)          |  April 30th, 2024             |
| Switches      | [DCS-7170-32CD](https://www.arista.com/en/support/advisories-notices/end-of-sale/19266-end-of-sale-of-the-arista-dcs-7170-32cd-series)<br>[DCS-7020SRG-24C2](https://www.arista.com/en/support/advisories-notices/end-of-sale/18884-end-of-sale-of-the-arista-dcs-7020srg-24c2-series)<br>[DCS-7280SR-48C6 & 7280TR-48C6](https://www.arista.com/en/support/advisories-notices/end-of-sale/17491-end-of-sale-of-the-arista-dcs-7280sr-48c6-and-dcs-7280tr-48c6-series)<br>[DCS-7280CR2-60 Series](https://www.arista.com/en/support/advisories-notices/end-of-sale/17490-end-of-sale-of-the-arista-dcs-7280cr2-60-series)<br>[DCS-7010T-48](https://www.arista.com/en/support/advisories-notices/end-of-sale/16538-end-of-sale-7010t-48)<br>      |    Varies by Device |


**New Releases** of Arista's device are listed below 

   |  Device       | More Information |  Release Date 
   | :-----------: | :-----------:    | :-----------:
   | Arista Multi-Domain Segmentaton Service  | [Arista MSS](https://www.arista.com/en/company/news/press-release/19297-pr-20240430)         | Q3 2024
   |  Arista 7130 Series             |  [Ultra Low Latency Network](https://www.arista.com/en/company/news/press-release/18273-pr-20231011)  | Q4 2023
   |  Arista AGNI    |   [AI Driven Network Identity](https://www.arista.com/en/company/news/press-release/17244-pr-20230424)                | Q2 2023 
   | Arista CV UNO  | [CloudVision Universal Network Observability](https://www.arista.com/en/company/news/press-release/19195-pr-20240305)  | Q1 2024

---

# *Feel Free to Reach Out To Us For Your Network Needs* 
<figure markdown>
![Image Placement](img/pictureOfNetworks.jpeg){: style="height:300px;width:800px"}  
    <figcaption></figcaption>
</figure>
We thank you for taking the time to read out newsletter today. Feel free to reach out to your SE or ASE for more information or questions regardsing your network operations. Until next month, have a good one! 



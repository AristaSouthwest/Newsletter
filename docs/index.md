 ![Image Placememt](img/Arista_Logo_copy.png)


# Arista August Southwest Region Newsletter

Welcome to the August 2024 newsletter for Arista customers in the U.S. Southwest Region!
 
We welcome your feedback on the newsletter. If you have any ideas on what you want to see, please reach out to southwest@arista.com.

---

## **Transforming Connectivity: Introducing Arista's Modern WAN Routing System for SD-WAN 2.0**
By: Keith Huynh, Systems Engineer Southwest Region

As we navigate the ever-evolving landscape of networking, it's essential to recognize that while SD-WAN is not a new concept, Arista is redefining its potential with our cutting-edge, standards-based solutions. Here's a quick update on how we're leading the way.  

Revolutionizing SD-WAN with Standards-Based Innovation: SD-WAN has been a game-changer in networking for years, offering flexibility and cost savings. However, what sets Arista apart is our commitment to building on open standards, ensuring interoperability, and future-proofing your investments. Our Modern WAN Routing System leverages industry-standard protocols to create a robust and adaptive network fabric.  

Key Highlights of Arista's SD-WAN 2.0:

- Seamless Connectivity: Our WAN Routing System connects enterprise branches, data centers, and head offices across diverse regions using the best available paths tailored to specific applications.  
- CloudVision Pathfinder: This centralized service ensures efficient path computation, enhancing performance and reliability.
- Dynamic Path Selection: By using Dynamic Path Selection (DPS), our system forwards application traffic over the most optimal path, whether MPLS or the internet, based on real-time conditions.  
- Enterprise-Grade Hardware: Our solution is built on secure, enterprise-grade hardware powered by Arista EOS and secure boot technology, ensuring robust performance and security.

Adaptive Virtual Topology (AVT): Building on DPS, our AVT technology dynamically selects paths, ensuring that critical and latency-sensitive applications receive the best possible performance. This adaptability is crucial in today's fast-paced digital environment.  

Standards-Based Approach: Our emphasis on using open standards means that our solutions integrate seamlessly with existing infrastructures and are prepared for future advancements. This approach not only protects your investment but also simplifies network management and scalability.

Get In Touch: For more detailed information on our Modern WAN Routing System, reach out to your local account manager or systems engineering team. They are ready to provide insights and answer any questions you may have.

Links for additional information:  
[Dynamic Path Selection](https://www.arista.com/en/cg-veos-router/veos-router-dynamic-path-selection)  
[CloudVision](https://www.arista.com/en/support/toi/eos-4-30-0f/17496-wan-routing-system-adaptive-virtual-topology?tmpl=component&format=pdf)
[AWE 7200R Datasheet](https://www.arista.com/assets/data/pdf/Datasheets/AWE-7200R-Datasheet.pdf)  

---

## **VARP (Virtual Address Resolution Protocol)** 
By: Steven King, Systems Engineer Southwest Region

VARP is also called Layer-3 Anycast Gateway and is very simple to deploy. It is completely standards-based, and provides Active/Active behavior that HSRP and VRRP cannot replicate. Packets received on a VARP address are forwarded to the next hop destination on the same switch so that traffic does not need to traverse the inter-switch link.  This reduces latency and unnecessary load on switches. 

<figure markdown>
![Image Placement](img/AugustNewsletter_Pic1.png)
    <figcaption>  </figcaption>
</figure>

VARP works by responding to ARP requests for configured IP addresses with a configured virtual MAC address.  In the example below based off of your “segment” deployment diagram, two switches configured with VARP are providing a redundant first hop gateway to the downstream host, which resides in VLAN 1. Both switches respond to the host’s ARP request.  

<figure markdown>
![Image Placement](img/AugustNewsletter_Pic2.png)
    <figcaption> </figcaption>
</figure>

An important item to note is that outside of ARP, traffic sent is not sourced from the virtual MAC address configured for VARP, but the switch’s system MAC address instead.  To illustrate this point, consider the example below:  

<figure markdown>
![Image Placement](img/AugustNewsletter_Pic3.png){: style="height:300px;width:700px"}
    <figcaption> </figcaption>
</figure>

Two host machines are in two different VLANs with the switch acting as their default gateway, configured with VARP.  

1) HOST 1 in VLAN 172 sends an ICMP ECHO request to Host 2 in VLAN 99; the destination MAC is that of its gateway residing on the switch, provided by the VARP virtual MAC address.  

2) As the switch routes the request to HOST 2 in VLAN 99, the source MAC is not the virtual MAC address provided by VARP, but the switch’s system MAC address.  


Links for more information are below:  
[Arista EOS Virtual ARP (VARP) Behind the Scenes](https://blog.ipspace.net/2013/06/arista-eos-virtual-arp-varp-behind/)  
[Active-active router redundancy using VARP](https://arista.my.site.com/AristaCommunity/s/article/active-active-router-redundancy-using-varp)  


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
   | __EOS__           | 4.31.3.1M <br>4.30.7M <br>4.31.4M<br>4.29.4.2M<br>4.32.1F<br>     | July 17th, 2024 <br>July 8th, 2024<br>July 5th, 2024<br>June 25th, 2024<br>June 6th, 2024<br>
   | __CVP__           | 2024.2.0 <br>2024.1.2<br>     | July 26th, 2024 <br>May 10th, 2024<br>
   | __DMF__           | 8.6.0         | July 9th, 2024
   | __WLAN__ <br>CV-CUE<br>Wireless Manager<br> | <br>13.0.0-67<br>17.0.0<br>       | <br>December 15th, 2022<br>May 10th, 2023<br>
   | __Arista NDR__         | 5.1.2         | February 15th, 2024
   | __TerminAttr__    | 1.32.1        | June 13th, 2024


---

## __*Software Advisories*__
Below is a list of advisories that are announced by Arista. To view more details on the specific advisories, please click the links in the middle boxes.

| Name          | Advisory Link           | Date of Advisory Notice  |
| :-----------: |:-------------:| :-----:|
| __EOS in 802.1X mode__   | [Security Advisory 0103](https://www.arista.com/en/support/advisories-notices/security-advisory/19917-security-advisory-0103) | July 23rd, 2024
| __EOS with MACsec and egress ACLs__   | [Security Advisory 0102](https://www.arista.com/en/support/advisories-notices/security-advisory/19908-security-advisory-0102) | July 23rd, 2024
|  __RADIUS Protocol__   | [Security Advisory 0101](https://www.arista.com/en/support/advisories-notices/security-advisory/19905-security-advisory-0101)  | July 9th, 2024   |
| __OpenSSH__    | [Security Advisory 0100](https://www.arista.com/en/support/advisories-notices/security-advisory/19904-security-advisory-0100) |   July 8th, 2024             |
| __EOS with OpenConfig__              |  [Security Advisory 0099](https://www.arista.com/en/support/advisories-notices/security-advisory/19862-security-advisory-0099)             | July 2nd, 2024       |
| __WIPS feature in CV-CUE__    | [Field Notice 0083](https://www.arista.com/en/support/advisories-notices/field-notice/19902-field-notice-0083)               | July 9th, 2024             |

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



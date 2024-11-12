 ![Image Placememt](img/Arista_Logo_copy.png)


# Arista November Southwest Region Newsletter

Welcome to the November 2024 newsletter for Arista customers in the U.S. Southwest Region!
 
We welcome your feedback on the newsletter. If you have any ideas on what you want to see, please reach out to southwest@arista.com.

---

## **Interface Configuration Made Easy with Quick Actions**
By: Alex Bojko, Advanced Services Engineer, Southwest Region

Configuring network devices can prove to be a tedious task. CloudVision Studios was introduced with the aim of easing device configuration hardships by providing a simple to navigate interface for device provisioning. By leveraging Studios, network engineers can configure a large subset of devices without ever typing in a single line of CLI. At Arista, we are constantly improving the functionality of CloudVision, and Studios, being a feature within CloudVision, is no exception. We are constantly reimagining device provisioning methods, with our latest improvement coming in the form of a feature called "Quick Actions."  

The Access Interface Configuration Quick Action allows network operators to view their switch in CloudVision, displayed as an illustration of the front panel of the device.   



<figure markdown>
![Image Placement](img/Access Interface Config Quick Action Image.png)
    <figcaption> Front Panel Illustration </figcaption>
</figure> 


From here, the operator can select as many interfaces as required, and dynamically assign "Port Profiles" to the interfaces.   


**NOTE:** A Port Profile is a custom made profile intended to group common interface configuration settings into one location. For example, you can create a WIreless Access Point - Port Profile that sets the correct type of switchport, adds a description, adds any required vlans, and sets the speed, MTU, PTP settings, 802.1X configuration, PoE settings, and more. 

After assigning a port profile to an interface or subset of interfaces the network operator submits their change. The configuration parameters defined within the profile are leveraged to generate CLI configuration for the selected interfaces, which is then dynamically applied to each interface via a Change Control.  

Furthermore, an operator can select specific interfaces and simply add a vlan to them, making day 2 tasks easy for network operators of all skillsets.   

To learn more about the Access interface Configuration Quick Action, click the link below:   
[Quick Action Configuration](https://www.arista.io/help/articles/cHJvdmlzaW9uaW5nLnN0dWRpb3MuQWxsLmJ1aWx0SW4uYWNjZXNzLWludGVyZmFjZQ==)  

---

## **CloudVision Series Part 1: Stay Aware of Abnormal Network Behavior with Event Alerts** 
By: Akashdeep Takhar, Advanced Services Engineer, Southwest Region
 
Image this scenario, which has unfortunately occurred to many network operators. Traffic loss across the network has significantly impacted end hosts. Neighboring devices cannot connect with their peers, perhaps a physical port is down. End users that depend on these networks are now complaining that they cannot connect to their applications, many tickets are created, a nightmare of stress hinders everyone…..and the network team was informed of all this chaos unexpectedly without any warning. Event notifications system can assist in alerting your team for unforeseen circumstances, such as the ones discussed. This is where CloudVision’s Event Notification tool can help your team!  

The Event Notification tool is essential to use when utilizing CloudVision. Event Notifications communicate with 3rd party team collaboration tools such as Microsoft Teams, Slack, Google Chat, etc. via webhooks to send alerts directly to your team of desired destination. Not only is the team aware of anomalies within the Network as they occur, the team can also set threshold parameters with metrics to determine appropriate times to receive alerts. In this two part series, we’ll look at where to navigate to configure event notifications messages. Next month, we’ll show how to set threshold metrics to trigger the notifications to send messages.  

<figure markdown>
![Image Placement](img/Akash_Newsletter_Events1.png)
    <figcaption> Direction to navigate towards the Event Notification section </figcaption>
</figure> 

<figure markdown>
![Image Placement](img/Akash_Newsletter_Events2.png)
    <figcaption> Open the platform section </figcaption>
</figure> 

Start by navigating to the “Event” tab on the CloudVision portal on the left hand side of the page. Note that the pictures shown are of the latest version of CloudVision. If you currently run the previous version’s UI, the “Events” tab should be shown on top of the page.   

Upon landing onto the “Events” tab, navigate the mouse to the top right and click on “Event Notifications”. This will bring you to the section where you can configure the platform to receive notifications upon. How exactly does CloudVision communicate to these 3rd party platforms? This is accomplished via Webhooks. Webhooks use APIs to send communication data between the two tools. Webhook are created by the 3rd party platform and are unique for where it is sending API calls to. Each platform has a simple guide on generating the Webhook for CloudVision to use. Upon generating the Webhook, you can simply paste it to CloudVision and begin to send test messages.  

<figure markdown>
![Image Placement](img/Akash_Newsletter_Events3.png)
    <figcaption> Click on Receivers Tab </figcaption>
</figure> 

Under the “Receivers tab”, create a “Receiver” to inform CloudVision where to send the alert towards. Although the Webhook is recorded within the “Platform” tab, the “Receiver” tab finalizes the setting for CloudVision to recognize the receiving location.  

By configuring Event Notifications, your team will be aware of ongoing concern within the Network. Rather than logging in to constantly monitor the network, CloudVision can help automate the monitoring task by sending alerts for abnormal behavior within the network fabric. Not only would this allow the team to quickly identify the matter, this would also allow the team to receive the issue faster than the end hosts bugging you about the issue. Contact your SE or ASE to receive help on setting up Event Notifications today!  
  

Links for additional information on Events:  
[Accessing Events](https://www.arista.com/en/cg-cv/cv-accessing-events)  
[Additional Events App Information](https://www.arista.com/en/cg-cv/cv-events-app)  
[CloudVision Events Getting Started Video](https://www.youtube.com/watch?v=dxy0YSyvbkE) 

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
   | __EOS__           | 4.30.8.1M <br> 4.33.0F <br>4.32.2.1F <br>4.29.7.1M <br>4.31.5M<br>4.30.8M<br>    | October 30th, 2024 <br> October 10th, 2024 <br>October 2nd, 2024 <br>September 27th, 2024<br>September 26th, 2024<br>September 26th, 2024<br>
   | __CVP__           | Portal 2024.3.0 <br> Portal 2024.2.1 <br>Appliance 6.0.7<br> Sensor 1.0.0 <br>    | October 21st, 2024 <br> October 15th, 2024 <br>September 18th, 2024<br> October 16th, 2024 <br>
   | __DMF__           | 8.4.4 <br>8.5.1<br>        | September 26th, 2024 <br>August 15th, 2024
   | __WLAN__ <br>CV-CUE<br>Wireless Manager<br> | <br>13.0.0-67<br>17.0.0<br>       | <br>December 15th, 2022<br>July 12th, 2024<br>
   | __Arista NDR__         | 5.2.3         | August 2024
   | __TerminAttr__    | 1.34.2 <br> 1.31.7 <br> 1.28.8 <br>        | October 28th, 2024 <br> October 28th, 2024 <br> October 28th, 2024 <br>


---

## __*Software Advisories*__
Below is a list of advisories that are announced by Arista. To view more details on the specific advisories, please click the links in the middle boxes.

| Name          | Advisory Link           | Date of Advisory Notice  |
| :-----------: |:-------------:| :-----:|
|  __Edge Threat Management__   | [Security Advisory 0105](https://www.arista.com/en/support/advisories-notices/security-advisory/20454-security-advisory-0105)  | October 29th, 2024   |
| __CloudVision Appliance__   | [Security Advisory 0104](https://www.arista.com/en/support/advisories-notices/security-advisory/20405-security-advisory-0104) | September 24th, 2024
| __EOS in 802.1X mode__   | [Security Advisory 0103](https://www.arista.com/en/support/advisories-notices/security-advisory/19917-security-advisory-0103) | July 23rd, 2024
| __EOS with MACsec and egress ACLs__   | [Security Advisory 0102](https://www.arista.com/en/support/advisories-notices/security-advisory/19908-security-advisory-0102) | July 23rd, 2024
| __Mojo Identity ID__    | [Field Notice 0089](https://www.arista.com/en/support/advisories-notices/field-notice/20618-field-notice-0089)   | October 29th, 2024   |
| __WiFi AP Firmware__    |  [Field Notice 0088](https://www.arista.com/en/support/advisories-notices/field-notice/20438-field-notice-0088)  | October 23rd, 2024   |
| __Zero Touch Provisioning__    |  [Field Notice 0087](https://www.arista.com/en/support/advisories-notices/field-notice/20418-field-notice-0087)  | October 10th, 2024   |
| __Wi-Fi Integration with WLAN Controllers__         |  [Field Notice 0086](https://www.arista.com/en/support/advisories-notices/field-notice/20411-field-notice-0086) | October 1st, 2024    |



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
| Software      | [EOS 4.27 Series](https://www.arista.com/en/support/advisories-notices/end-of-support/20174-end-of-software-support-for-eos-4-27) | August 27th, 2024    |
| Module        | [7500R2 Series Linecards](https://www.arista.com/en/support/advisories-notices/end-of-sale/18886-end-of-sale-of-the-arista-7500r2-series-line-cards) | December 20th, 2023    |
| Access Points | [Arista 802.11ac Wave 2 Devices](https://www.arista.com/en/support/advisories-notices/end-of-sale/14911-end-of-sale-of-arista-802-11ac-wave-2-devices)      |  June 30th, 2022 |
| DMF           | [Analytics Node DCA-DM-AA3](https://www.arista.com/en/support/advisories-notices/end-of-sale/20142-end-of-sale-end-of-life-for-arista-analytics-node-appliance-dca-dm-aa3)          |  August 3rd, 2024             |
| DMF           | [Pluribus NVOS, UNUM, Freedom 9000](https://www.arista.com/en/support/advisories-notices/end-of-sale/20133-end-of-sale-pluribus-nvos-unum-freedom-9000-series)          |  August 2nd, 2024             |
| Switches      | [DCS-7130-96S Series](https://www.arista.com/en/support/advisories-notices/end-of-sale/20381-end-of-sale-of-the-arista-dcs-7130-96s-series)<br>[DCS-7170 and 7170B Series](https://www.arista.com/en/support/advisories-notices/end-of-sale/19846-end-of-sale-of-the-arista-7170-and-7170b-series)<br>[DCS-7130B-32QD](https://www.arista.com/en/support/advisories-notices/end-of-sale/19845-end-of-sale-of-the-arista-dcs-7130b-32qd-series)<br>[DCS-7170-32CD](https://www.arista.com/en/support/advisories-notices/end-of-sale/19266-end-of-sale-of-the-arista-dcs-7170-32cd-series)<br>[DCS-7010T-48](https://www.arista.com/en/support/advisories-notices/end-of-sale/16538-end-of-sale-7010t-48)<br>      |    Varies by Device |


**New Releases** of Arista's device are listed below 

   |  Device       | More Information |  Release Date 
   | :-----------: | :-----------:    | :-----------:
   | Arista Multi-Domain Segmentaton Service  | [Arista MSS](https://www.arista.com/en/company/news/press-release/19297-pr-20240430)         | Q3 2024
   |  Arista 7130 Series             |  [Ultra Low Latency Network](https://www.arista.com/en/company/news/press-release/18273-pr-20231011)  | Q4 2023
   |  Arista AGNI    |   [AI Driven Network Identity](https://www.arista.com/en/company/news/press-release/17244-pr-20230424)                | Q2 2023 
   | Arista CV UNO  | [CloudVision Universal Network Observability](https://www.arista.com/en/company/news/press-release/19195-pr-20240305)  | Q1 2024

---

## __**We're Hiring!**__

Our team is looking to hire the following roles, located in Southwest area:

*Network Systems Engineer*  
[Phoenix SE Role, Click Here](https://www.smartrecruiters.com/AristaNetworks/743999994606279-network-systems-engineer-pre-sales-)    
[Los Angeles SE Role, CLick Here](https://www.smartrecruiters.com/AristaNetworks/744000011382271-network-systems-engineer-pre-sales-)

*Network Advanced Services Engineer*  
[Southwest ASE Role, Click Here](https://www.smartrecruiters.com/AristaNetworks/744000000783368-network-advanced-services-engineer)



---
# *Feel Free to Reach Out To Us For Your Network Needs* 
<figure markdown>
![Image Placement](img/pictureOfNetworks.jpeg){: style="height:300px;width:800px"}  
    <figcaption></figcaption>
</figure>
We thank you for taking the time to read out newsletter today. Feel free to reach out to your SE or ASE for more information or questions regardsing your network operations. Until next month, have a good one! 



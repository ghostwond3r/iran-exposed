English | Persian
<br>

# Behnama Leak Explained

<br>

## What is FANAP?

- Established with the investment of Pasargad Financial Group
- Primary mission was to design and prepare a native Iranian banking solution
- Funded Arvan Cloud.

<br>

But they expended they activities way more further than that:

    BehNama - Video surveillance using facial recognition (implemented in all Pasargad Bank)
    BehYab - Car GPS and tracking system
    BehKhan - Car plate recognition system (hijab alert)
    BehCard - Face recognition system for printing ID card

<br>

## Connected to the regime

The SSO platform used by the Regime to authenticate user online, are connected to FANAP system that make usage of an API, compiling each details of your life, to classify who has rights to access a service, or not, but also to build a floating card beside your head for facial recognition.

The pod.ir API, access the same system as the SSO, and is also connected to Pasargad Bank. FANAP called it the Podium, and they owns it. Pod is  management platform for all kind of monitoring, people or, internet.

<br>

## Pasargad Financial Group

The Pasargad Financial Group is comprised of Pasargad Bank and several other companies, which operate in the areas of information technology, communications, electronic payment services, insurance, reinsurance, brokerages, heavy equipment leasing, commercial building leasing, construction, mining and industry, energy and other services. One of their companies is FANAP.

FANAP also have multiple sub companies, and has developed everything in order to deploy the National Information Network (intranet).

Some companies owned by Pasargad Financial Group:

    1.   Bank Pasargad
    2.   Middle East Mining and Mining Industries Holding
    3.   Pasargad Arian Information and Communications (FNAP)
    4.   Pasargad Insurance
    5.   Iranian Reinsurance Company
    6.   Pasargad Heavy Machinery and Equipment Leasing Company
    7.   Pasargad Leasing
    8.   Parsargad Arzesh Afarinan Company
    9.   Middle East Foundational Company
    10.  Pasargad Energy Development
    11.  Pasargad Bank Electronic Payments
    12.  Pasargad Currency Exchange and Services
    13.  Pasargad Bank Brokerage Services
    14.  Eighth Urban Development and Construction Company
    15.  Pasargad Mass Production
    16.  Pasargad Human Capital Research and Development Institution
    17.  Arian Investments (AICO)
    18.  Arian Engineering and Construction Management
    19.  Arian Pasargad Construction Management
    20.  Pars Arian Investments
    21.  Pasargad Bank Financial and Investment Services
    22.  Pasargad Bank Investments
    23.  Arian Construction (Modabberan)
    24.  Iran Credit Ranking Consulting
    25.  Arian Saman Construction
    26.  Pasargad Arian Logistics Services
    27.  Pasargad Financial Group Pension
    28.  Pasargad Commerce Development
    29.  Pasargad Tadbirgaran Company
    30.  Pasargad Future Commerce Management
    31.  Pasargad Group International Commerce Development and Expansion
    32.  Mana Iranian Renewal and Expansion Industries
    33.  Zarand Iranian Steel Company
    34.  Middle East Aftab Derakhshan (Shining Sun) Commerce
    35.  Iranian Sirjan Steel Company
    36.  Middle East Meyar Industrial Engineering Company
    37.  Pars Hafez Investments.

<br>

## Fannap-infrastructure

This division is in charge of developing multiple software, and here we exposed one of them. Behnama is a video surveillance system that operates on a Linux platform. It is primarily written in C++, PHP, and C. 

This system was initially deployed across all branches of Pasargad Bank, marking its first use. A standout feature of Behnama is its development for facial recognition capabilities, enhancing its surveillance effectiveness.

<br>

## Behnama

It is built on microservice architecture, it contains RTSP client, recording, web-app, webrtc, API, analyzer, Kafka, ONVIF, PostgressDB and influxDB services.

Some of their utilities:

    • Kafka from Apache, is a service likely used for real-time processing of video data from multiple sources.

    • Redis and Postgres services are likely used to store metadata or analysis results. They store information about when and where each face was detected, or they might store the facial recognition results.

    • ONVIF service and RTSP client are used to interact with IP cameras that support these protocols. They arr used to retrieve the video data    that is processed by the Kafka and Analyzer services.

    • The Jaeger, SeaweedFS, ELK stack, and Filebeat services are likely used for system monitoring and debugging. They are used to trace system   activity, store system data, log system events, and ship logs to a centralized location for analysis.

The software seems to connect to vCenter, a centralized management application and framework that acts as a proxy for managing VMware vSphere environments. They are also connected to a monitoring panel owned by Net Negar (netnegar.io) that seems adapted for the National internet project.

The software use an API to connects to pod.ir by MQTT protocol. Pod is a grand plan to create an infrastructural and comprehensive platform designed and developed by Fanap, in order to develop sub-platforms and online businesses. This platform is connected to Pasargad Bank and all the businesses developed in it are connected to the digital platforms of this bank. The Pod API documentation include a whole section for facial recognition. https://accounts.pod.ir/apidocs/

| See ANNEXE A to understand what is the Pod API.

<br>

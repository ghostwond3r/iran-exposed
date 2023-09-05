English | Persian
<br>

<p align="right">
<img src="https://github.com/NeverWonderLand/iran-exposed/assets/64184513/9cfe124c-6d1f-469a-a3a3-34a886e0e494" alt="9cfe124c-6d1f-469a-a3a3-34a886e0e494"
</p>

# Behnama Leak Explained

<br>

## What is FANAP?

- Established with the investment of Pasargad Financial Group
- Primary mission was to design and prepare a native Iranian banking solution
- Funded Arvan Cloud.

<br>

### Subsidiary companies of Fanap holding:

Pasargad Electronic Payment, Abr Arvan, Fanap Telecom, Kuknos (Phoenix), Adonis, Baran Telecom, Fanap Zirsakht (Fanp Infrastructure), Parsa, Lamasoo, Spara, Smilino, Datex, Fanap Plus, Fanap Tech, Fanap Soft, Zitel, Sepandar, Alfa, Rajman, Shenasa, Dotin, Podro.

<br>

## Fannap-infrastructure

This division is in charge of developing multiple software, and here we exposed one of them. Behnama is a video surveillance system that operates on a Linux platform. It is primarily written in C++, PHP, and C. 

This system was initially deployed across all branches of Pasargad Bank, marking its first use. A standout feature of Behnama is its development for facial recognition capabilities, enhancing its surveillance effectiveness.

But they expended they activities way more further than that:

    BehNama - Video surveillance using facial recognition (implemented in all Pasargad Bank)
    BehYab - Car GPS and tracking system
    BehKhan - Car plate recognition system (hijab alert)
    BehCard - Face recognition system for printing ID card
    
<br>

## Pasargad Financial Group

The Pasargad Financial Group is comprised of Pasargad Bank and several other companies, which operate in the areas of information technology, communications, electronic payment services, insurance, reinsurance, brokerages, heavy equipment leasing, commercial building leasing, construction, mining and industry, energy and other services. One of their companies is FANAP.

FANAP also have multiple sub companies, and has developed everything in order to deploy the National Information Network (intranet).

| To see all companies owned by them please see ANNEXE A.

<br>

## Behnama

The software is built on microservice architecture and contains components like: RTSP client, recording, web-app, webrtc, API, analyzer, Kafka, ONVIF, PostgressDB and influxDB services.

Some of their utilities:

    • Kafka from Apache, is a service likely used for real-time processing of video data from multiple sources.

    • Redis and Postgres services are likely used to store metadata or analysis results. They store information about when and where each face was detected, or they might store the facial recognition results.

    • ONVIF service and RTSP client are used to interact with IP cameras that support these protocols. They arr used to retrieve the video data    that is processed by the Kafka and Analyzer services.

    • The Jaeger, SeaweedFS, ELK stack, and Filebeat services are likely used for system monitoring and debugging. They are used to trace system   activity, store system data, log system events, and ship logs to a centralized location for analysis.

The software seems to connect to vCenter, a centralized management application and framework that acts as a proxy for managing VMware vSphere environments. They are also connected to a monitoring panel owned by Net Negar (netnegar.io) that seems adapted for the National internet project.

The software use an API to connects to pod.ir by MQTT protocol. Pod is a grand plan to create an infrastructural and comprehensive platform designed and developed by Fanap, in order to develop sub-platforms and online businesses. This platform is connected to Pasargad Bank and all the businesses developed in it are connected to the digital platforms of this bank. The Pod API documentation include a whole section for facial recognition. https://accounts.pod.ir/apidocs/

| See [ANNEXE B](https://github.com/NeverWonderLand/iran-exposed/blob/main/ANNEXE_B.md) to understand what is the Pod API.

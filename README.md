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

| To see all companies owned by them please see [ANNEXE A](https://github.com/NeverWonderLand/iran-exposed/blob/main/ANNEXE_A.md).

<br>

## Behnama

The initial company that developed Behnama software was Behpooyesh.

They was specialized in:

    • Software production
    • Video Surveillance
    • GIS
    • Digital Signage
    • License Place Recognition
    • Image Processing

<br>

> After getting acquainted with Fanap company, it was then included in the group of holding companies of Fanap. 
<br>

The software is built on microservice architecture and contains components like: 

    - RTSP 
    - Recording
    - Webrtc
    - API
    - Analyzer
    - Kafka
    - ONVIF
    - PostgreSQL
    - InfluxDB

<br>

The software seems to connect to vCenter, a centralized management application and framework that acts as a proxy for managing VMware vSphere environments. They are also connected to a monitoring panel owned by Net Negar (netnegar.io) that seems adapted for the National internet project.

<br> 

## Pod

The software use an API to connects to pod.ir by MQTT protocol. 

Pod is a grand plan to create an infrastructural and comprehensive platform designed and developed by Fanap, in order to develop sub-platforms and online businesses. 

This platform is connected to Pasargad Bank and all the businesses developed in it are connected to the digital platforms of this bank. 

The Pod API documentation include a whole section for facial recognition. https://accounts.pod.ir/apidocs/

| See [ANNEXE B](https://github.com/NeverWonderLand/iran-exposed/blob/main/ANNEXE_B.md) to understand what is the Pod API.

<br>

## SHAHKAR

| The Pod API system is tied to SHAHKAR as you can see [here](https://accounts.pod.ir/apidocs/#/Verifications/manualShahkarVerify).

**SHAHKAR System** – A data warehouse which stores information about all mobile subscribers in Iran to check the “validity of users” and prohibit any registration attempt if the CRA determines the attempt to be invalid. The purpose of the SHAHKAR system is to notify the CRA of users attempting to change to a different service provider, update their subscription information or change their phone number. 

SHAHKAR prevents users from acquiring new mobile accounts with multiple service providers. This implies that Iran maintains a 1:1 mapping of a user to a SIM profile to simplify its ability to conduct surveillance operations. It provides the CRA with the ability to immediately cancel a user request for a new mobile account or make changes to existing accounts.

| For more informations about SHAHKAR system please read this [article](https://citizenlab.ca/2023/01/uncovering-irans-mobile-legal-intercept-system/).

<br>

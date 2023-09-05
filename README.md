# Behnama Leak Explained
    
[What is Fanap?](https://github.com/NeverWonderLand/iran-exposed/blob/main/README.md#what-is-fanap)

[Fanap-Infrastructure](https://github.com/NeverWonderLand/iran-exposed/blob/main/README.md#fannap-infrastructure)

[Pasargad Group](https://github.com/NeverWonderLand/iran-exposed/blob/main/README.md#pasargad-financial-group)

[Behnama](https://github.com/NeverWonderLand/iran-exposed/blob/main/README.md#behnama)

[Pod](https://github.com/NeverWonderLand/iran-exposed/blob/main/README.md#pod)  

[SHAHKAR](https://github.com/NeverWonderLand/iran-exposed/blob/main/README.md#shahkar)

[Machine Learning](https://github.com/NeverWonderLand/iran-exposed/blob/main/README.md#machine-learning)

[National Information Network](https://github.com/NeverWonderLand/iran-exposed/blob/main/README.md#the-link-with-the-national-information-network)

<br>

> There is no databases with the faces of people that have been leaks, only the code itself.

<br>

<p align="center">
<img src="https://cybershafarat.com/wp-content/uploads/2023/08/IMG_20230828_052706_287.jpg" alt="IMG_20230828_052706_287.jpg"
</p>

<br><br>
    
## What is FANAP?

- Established with the investment of Pasargad Financial Group
- Primary mission was to design and prepare a native Iranian banking solution
- Funded Arvan Cloud.

### Subsidiary companies of Fanap holding:

Pasargad Electronic Payment, Abr Arvan, Fanap Telecom, Kuknos (Phoenix), Adonis, Baran Telecom, Fanap Zirsakht (Fanp Infrastructure), Parsa, Lamasoo, Spara, Smilino, Datex, Fanap Plus, Fanap Tech, Fanap Soft, Zitel, Sepandar, Alfa, Rajman, Shenasa, Dotin, Podro.

<br>

<p align="center">
<img src=https://github.com/NeverWonderLand/iran-exposed/assets/64184513/b5a36fc7-5cef-43c3-8f53-26c31563ae34" alt="b5a36fc7-5cef-43c3-8f53-26c31563ae34"
</p>

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

The website was first registred on 31 JUL 2016.

    Name: Ali Asghar Rostami
    Company: Behpooyesh iranian asia 
    Email: h.rostami@behpooyesh.com

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

Behnama is not just a tool; it is a powerful instrument of surveillance. It is being actively used by the Iranian government, law enforcement agencies, and military personnel, marking a significant development in the country's surveillance capabilities.

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

Relationship between Iran’s Legal Intercept System Interfaces and Mobile Service Provider Systems along with examples of Legal Intercept System Commands that query user information and control services.

This, joint with the Behnama software, make a pure invasive system.

| For more informations about SHAHKAR system please read this [article](https://citizenlab.ca/2023/01/uncovering-irans-mobile-legal-intercept-system/).

<br>

## Machine Learning 

A machine learning model (AI) use by the analyzer for the facial recognition process has been identified.

The identification was found here:

    ANALYZER/CORE/PEOPLE_COUNTER/pycache/people_counter.cpython-37.pyc

> The model use is Yolov5 - Crowdhuman

> MFR model is also use (you can see it as well in some .pyc files)

<br>

## The link with the National Information Network

This is an important part to understand the real extend of the Behnama software. The facial recognition itself is relying on other crucial components of the future Iranian Intranet.

Abr Arvan, which presents itself as the first content delivery network in Iran, was launched in a conference titled “Explaining Strategies for Developing a Content Distribution Network in the Context of the National Information Network.”

The company started in 2014, with the aim of producing cloud technological products. The founding team consisted of four people, whose first acquaintance was formed in the World Skills Competition. These people were selected as the first team product in March 2015 in the Fanap Innovation Competition.

Abr Arvan had fundraised in two phases, both of which were carried out by FANAP. Abr Arvan has always been a subset of FANAP holding, and one of its main companies.

FANAP holding was founded on December 15, 2005, through an investment by Pasargad Financial Group (Pasargad Bank). Pasargad Bank was also founded in 2005, with an official license from the Central Bank of Iran, and a 350 billion tomans fund which was fully paid.

Pasargad Financial Group has more than 22 holdings and large companies, many of which are chaired by Ghasemi, including FANAP. FANAP holding has more than thirteen subsidiary companies.

Mostafa Naghipourfar was the chairman of Abr Arvan from the company’s founding in 2015 until 2018. Besides being the first chairman of Abr Arvan and one of its founders, he is one of the founders of FANAP holding. 

He is now the council to the CEO of FANAP holding, and the secretary of the Iranian Association of New Financial Technologies (Fintech). Naghipourfar has been the CEO and chairman of more than 10 companies so far, some of which were subsets of FANAP holding, such as Baran Telecom, Inc.

In 2021, Arvan engaged in a contract with Ministry of ICT of Iran on Iran Cloud project. The project is set to deploy National Information Network, a network that allows the Iranian government to cut off Iranian users' access to the internet and provide them only domestic networks.

> For more details about this please read this [article](https://en.radiozamaneh.com/31799/).

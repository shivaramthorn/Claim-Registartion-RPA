# Claim-Registration-RPA
Insurance Claim Registartion

## Problem Statement
Many insurance companies are struggling to process large number of claim requests, as this is a repeated task for the customer support executives for processing big set of claims.To solve this problem we are using RPA automation to register multiple  claims for immediate processing in general insurance(Motor vehicle,Health,Property).

## Abstract
The automated process, is a trending technology to reduce human repeated works like data entry. The insurance company has to register a claim, for the requested insurance policy from the insurer holder and also has different registration processes according to the insurance applied by the client.
This project is based on registering the request for claiming Motor policies in general insurance and other polices in general insurance, RPA uses the policy number as a key input to proceed which are provided by the insurers so it can be
accessed through an excel file, hence each policy can get registered if it is a valid request, after the verification of various factors (like black listing of vehicles, clients, engines & chassis) and Estimating the Eligiblity to claim the policy is calculated using the sum insured,Claimed amount,Bill Amount & NCD. All these processes are automated to have time efficient process to satisfy the client
needs.

## Modules
- Image Scraping               [Shivaram B]
- Motor Policy Registration    [Shivaram B]
- Cross Product Registration   [Shivaram B]
- Health Policy Registration   [Aishwarya R]
- Property Policy Registration [Dini Kokila K]

## Image Scraping
The Bill from pannel workshop for Motor Vehicles Damages and The Hospital Bill are Image scraped and store the Total Amount from the bill in the Input excel file.

## Motor Policy Registration
The input policy no from the excel file is fetched and it is checked for Black list(Insurer Holder,Engine No,Vehicle No,Chasis No) from another excel file which contains the Policy details and Black list details. The Verified details will be sent to customer as a mail if the policy holder has a Black list then Detials of Balck list will be sent as mail to the customer.

## Cross Product Registration
While Processing the Motor Policy registration the Bot checks for whether multiple policy like Personal accident is also requested or no, If personal accident policy also requested then the bot will process the perosnal accident policy while holding the Motor Registration policy. After completing the Personal accident policy registration the Holded Motor vehicle registration is continued.  The Verified details will be sent to customer as a mail if the policy holder has a Black list then Detials of Balck list will be sent as mail to the customer.

## Health Policy Registration
The input policy no from the excel file is fetched and it is checked for Black list(Insurer Holder) from another excel file which contains the Policy details and Black list details. If the health policy type is personal accident then the bot will check whether this policy number is processed in the Cross product registration. If it is processed in the cross product registration then it won't be processed in the Health Policy registration. The Verified details will be sent to customer as a mail if the policy holder has a Black list then Detials of Balck list will be sent as mail to the customer.

## Property Policy Registration
The input policy number is checked for separating the property policy no so that it can processed in different process that is after fetching the input policy no of property policy number it is checked for Black List(Insurer Holder) from another excel file which cotains the policy details and Black list details. Since the property policy requier manual verification from a customer executive to confirm the damage of the property the eligibe policy holder from the client request are listed in new excel file and the new excel file will be sent as mail to the customer executive who verify the property.

## Project Status
- Image Scraping (Working Successfully)
- Motor Policy Registration(90% Completed)
- Cross Product Registration((90% Completed)
- Health Policy Registration(90% Completed)
- Property Policy Registration(50% Completed)

## Pending Works
- Image Scraping (None)
- Motor Policy Registration (Mail Drafting)
- Cross Product Registration (Mail Drafting)
- Health Policy Registration (Mail Drafting)
- Property Policy Registration (Mail automation and Excel Automation)

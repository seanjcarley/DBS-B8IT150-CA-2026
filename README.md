# DBS-B8IT150-CA-2026

## Business Requirement
Develop a CRM to be used by a Toll Collection company. The system would have to manage data from multiple sources, and present it allowingcustomer service repshelp road users with any queries they have. Road users have multiple contact options (web, phone, etc…) and the system needs to be able to accommodate this. The Toll Collection company is operating the system on behalf of the Transport Agency, so reporting will also be needed to provide information on paid/unpaid tolls, volumes
The system should allow TCSP agents to retrieve teh relevant proof of the passage through the tolling point (images, date/time, vehicle registration number, vehicle class for applying appropriat charge, etc...), the means to correct any errors, system or human, to allow them assist the TRU with any queries they may contact about.

## Steakholders
- Transport Agency (TA)
- Toll Collection Provider (TCP)
- Customer Support Rep (CSR)
- Road User (RU)

## Overview
The TA will be the customer receiving the service provided by the TCP to collect and process tolls for journeys made by the RU through the tolled section of the applicable road infrastructure. The TCP's CSRs will use the system to provide this service and the TA will be able to view the status via reporting provided by the system.


## Non-functional Requirements
- low latency: CSR should be able to locate the information relating to the customer easily so as resolve any issues quickly minimising the time the RU spends on a call
- Data security: RU's data should only be shown when requested and to an authorised user
- Reporting: why do RU contact, what percentage of RUs pay without interaction, etc…
- Auditability: provide a transparent and reliable audit trail that can be used in any legal proceedings.
- Contact: allow data to be sent (securely) to RU (i.e. receipts, photographic proof...)
- Ease of use: minimise the amount of training time needed for CSR to use system
- Disaster Recovery: frequent back-ups to prevent the loss of data, and easy restore if/when required
- Comply with regulations and standards, for example (Payment Card Industry Data Security Standard (PCI DSS), General Data Protection Regulations(GDPR), etc… )
- Interoperability: integrate with other systems (eg: telephony, payments, etc…) 


## Functional Requirements
- Store all information in relation to the RUs interactions to db
- date and time of contact
- channel used for contact (phone, web, etc…)
- category of contact (payment, query…)
- change of status (paid, queried, error…)
- summary of interaction and resolution/further contact
- Provide the means to search for data relating to RU (using LPN/ref no)
- Provide the means for the CSR to input a summary of interaction with RU
- Provide the means for taking payments securely
- Provide automation where practical (automated invoice delivery/balance reminders, via email/SMS, etc…)

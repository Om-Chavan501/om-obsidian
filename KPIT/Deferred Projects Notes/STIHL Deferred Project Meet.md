Change Request and Maintainance
Change Request and Maintainance

OTX and ODX, DTC

Feature Extension
Bug Fixing
Change request

Or new feature scope is not changing complete architecture, it is a subset of the existing architecture.
Eg for this machine family

Backend java springboot
Frontend Angular

ODX - Storing ecu config and vehicle info 
OTX - ISO Std that our rte supports. It's sequencial execution of UDS Services
We have std protocol and properiety protocol that is specific to STIHL cutomer
Their next generation of machines are based on UDS compliance. Variety of protocols 
DDM - KPIT inhouse product, integrated with service tester, responsible for managing dependencies between hw, sw, ecus, releases/versions. Communicates with service tester
DDS - Diagnostic data store - storing vehicle info that is read out from the machine, stores snapshot data. service tester stores into dds, and it uses data from dds later on
LIMAS - KPIT Product - To managing licence related functionality of the tool, whether the particular user has valid license or not. Service tester connects with limas and does necesary info exchange to validate if user authorised or not. STandard implementation using STIHL requirements.
PDU API - Low level component, resp for establishing commn with vehicle interface, and resp for doing commn with vehicle, get info and read and send it to the service tester, but it is designed according to ISO standard. Along with some properietery communication protocols



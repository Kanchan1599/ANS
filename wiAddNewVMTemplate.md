# Add New VM Template

## Table of Contents

- [Changelog](#Changelog)
- [Introduction](#Introduction)
- [Purpose](#Purpose)
- [Scope](#Scope)
- [Steps](#Steps)
- [Prerequisites](#Prerequisties)
- [Template validation in vcenter](#Template-validation-in-vcenter)
- [Infrastucture(Image Mapping) in vRA](#Infrastucture(Image-Mapping)-in-vRA)
- [Apply Image in Blueprint](#Apply-Image-in-Blueprint)

## Changelog
  
| Version | Date       | Description      | Author       |
| ------- | ---------- | ---------------- | -------------|
| 0.1     | 27/09/2022 | Adding New VM Template In ANS-MAR & CLY  | Pardeshi Kanchan |

## Introduction

### Purpose
   
   The purpose of this document is to create step by step instructions for adding New VM Template in blueprints as per customer request.
### Scope

   Adding New VM Template in both ANS-MAR & ANS-CLY Environment. Notes- Customer may request addition of new VM Template in one site or both the sites.
   
## Steps

   There are three steps We need to perform-
   
   1. Template validation in vcenter
   
   2. Infrastucture(Image Mapping) in vRA
   
   3. Apply Image in Blueprint
   
## Prerequisites

  Prerequisites to Add New VM Templae.

  1. Access to respective tenants (eg-ans-mar-01 , ans-cly01) in VRA.

## Template validation in vcenter

 1. Customer should make new vm template available in vcenter. 

 2. All the changes or modifition to the template will be in customer scope.

 3. Root password on the template should be same as for the existing template.

## Infrastucture(Image Mapping) in vRA
    
 - For Adding new VM template in Blueprint, Log on to VRA Cloud Assembly.
 
 ![Figure 1](images/VMTemplate1.PNG)

 - For mapping of Image, Select Infrastucture Click on Image Mapping, And Add new image mapping
    
 ![Figure 1](images/VMTemplate2.PNG)

 - Give the Image Name and in Configuration select the region where image is availble and then in image we should select particular image and Click on create 
    
 ![Figure 1](images/VMTemplate3.PNG)

 - After Creation it will be visible in Image Mapping 

 ![Figure 1](images/VMTemplate4.PNG)

## Configure Image in Blueprint

 - To Configure Image go to Design, and select your blueprint and Add New image mapping under image variable.
    
 ![Figure 1](images/VMTemplate5.PNG)
 
 - Once blueprint is ready just go and create version of it and add proper description for it and click on check box of release version to catalog and click on create .
    
 ![Figure 1](images/VMTemplate12.PNG)
  
 - After creating version, then go to service broker 
    
  ![Figure 1](images/VMTemplate8.PNG)
  
 - Click on Content & Policies, then go to Content Sources
    
  ![Figure 1](images/VMTemplate9.PNG)
  
 - Just Validate it once and then Save & Import
    
  ![Figure 1](images/VMTemplate10.PNG)
  
 - Once it gets Validated then go to catalog and open catalog in which you have created version and then we will be able to see image in that catalog, Once done with all process once deploy and check whether its working properly.
    
  ![Figure 1](images/VMTemplate11.PNG)
  
## Note

  - Once proper testing has to be done for vm provisioning using that template in DEV blueprint only

  - If all testing are ok, then only that tempalte can be made available in PRD blueprint..
  
  - Without end to end testing of new template in DEV blueprint it cant be deployed in PRD blueprint

 
  

      


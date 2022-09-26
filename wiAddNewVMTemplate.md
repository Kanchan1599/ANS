# Updating Puppet Roles/Tags

## Table of Contents

- [Changelog](#Changelog)
- [Introduction](#Introduction)
- [Purpose](#Purpose)
- [Scope](#Scope)
- [Steps](#Steps)
- [Prerequisites](#Prerequisties)
- [Template validation in vcenter](#Template-validation-in-vcenter)
- [Infrastucture(Image Mapping) in vRA](#Infrastucture(Image-Mapping)-in-vRA)

## Changelog
  
| Version | Date       | Description      | Author       |
| ------- | ---------- | ---------------- | -------------|
| 0.1     | 21/09/2022 | Updating Puppet Roles In ANS-MAR & CLY  | Pardeshi Kanchan |

## Introduction

### Purpose
   
   The purpose of this document is to create step by step instructions for adding New VM Template in blueprints as per customer request.
### Scope

   Adding New VM Template in both ANS-MAR & ANS-CLY Environment. Notes- Customer may request addition of new VM Template in one site or both the sites.
   
## Steps

   There are two places where we have to make changes-
   
   1. Template validation in vcenter
   
   2. Infrastucture(Image Mapping) in vRA
   
   3. Apply Image in Blueprint
   
## Prerequisites

  Prerequisites to Add New VM Templae.

  1. Access to both tenants ans-mar-01 & ans-cly01 in VRA.
  
## Step 1

## Template validation in vcenter

- Step 1.1

  - customer should make new vm template available in vcenter. 
    
- Step 1.2

  - all the changes or modifition to the template will be in customer scope.
    
- Step 1.3

  - root password on the template should be same as for the existing template.

## Step 2

## Infrastucture(Image Mapping) in vRA

- Step 2.1
    
    - For Adding new VM template in Blueprint , Log on to VRA Service Broker
  
 
  

      


# Updating Puppet Roles/Tags

## Table of Contents

- [Changelog](#Changelog)
- [Introduction](#Introduction)
- [Purpose](#Purpose)
- [Scope](#Scope)
- [Steps](#Steps)
- [Prerequisites](#Prerequisties)
- [Infrastucture(Image Mapping) in vRA](#Infrastucture(Image Mapping) in vRA)

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
   
   1. Infrastucture(Image Mapping) in vRA
   
   2. Apply Image in Blueprint
   
## Prerequisites

  Prerequisites to Add New VM Templae.

  1. Access to both tenants ans-mar-01 & ans-cly01 in VRA.
  
## Step 1

## Infrastucture(Image Mapping) in vRA


  ### Note:
 
    - Before Starting below steps need to check whether VM Template is available in vcenter or not if its available then start with adding of new VM template.
  
  - Step 1.1
      


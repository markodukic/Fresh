---
title: Feature
keywords: usecase,use case, user stories, feature, epics, scenarios, nhsnumber
tags: [foundations,use_case,user stories, epics, scenarios]
sidebar: engage_sidebar
permalink: engage_feature.html
summary: "Feature contains user stories to search for a Care Connect FHIR&reg; Profile."
---


## title: Hospital discharge/encounter ##

{% include callout.html content="
scenario: >-
	<b>Scenario:</b><br>'Michael is to be discharged from hospital, with a care plan, and Dr. Hospital prepares his discharge summary. Dr. Hospital reconciles and reviews Michael’s discharge medications and produces a reconciled list of discharge medications. This includes hospital managed medication, new medications commenced during the hospital admission, Michael’s own over-the-counter medication, ongoing medication from the GP or other sectors.' 
"%}


<img src="images/use_cases/michaels_story-epic_1.jpg" style="width:100%;max-width: 100%;"> 


{% include callout.html content="
conversations: >-
	<b>Further Conversations:</b><br>
	This example refers to the reconciliation being performed by the doctor. The stories reflect this scenario and don’t explore the other cases where the reconciliation is performed by a technician or a pharmacist. This could be significant given that reconciliation by a technician when not validated by a pharmacist would include additional workflow for review.
"%}


### EPIC: Reconcile the patient’s drug chart for discharge ###

| User Story    | Profile     | Search     |
| :--- |--------------: |
| Story: >-
	As a clinician (hospital services) I want to ‘stop’ medication that is present on the patient’s drug chart because a drug is no longer being taken by the patient or I do not consider it necessary to 'take out'. | Post: POST <br>MedicationRequest | Search: patient |


# GTI - JIT STUDENT FLOW TO INITIATE CHAT PROCESS

This document outlines the process for how a student can initiate a chat for a specific unit they enrolled in under GTI.

We utilised the GTI reference APIs to retrieve the necessary information required to initiate the chat session.

## Reference Link

<https://app.axcelerate.com/apidocs/home/index>

## STUDENT LOGIN

Students can log in using their Contact ID (e.g., 14149898).

This Contact ID is passed as a parameter to the API to retrieve the student's details.

When the student enters their contact ID, a unique OTP is generated and sent to their email address. The email address is retrieved from the EMAILADDRESS field in the response returned by the Get Student Details API.

### URL to get student details

<https://globaltraining.app.axcelerate.com/api/contact/{contactId}>

### Example Response - Student Details

    {
        "CONTACTID": 14149898,
        "USERID": 2990980,
        "GIVENNAME": "Devi",
        "TITLE": null,
        "MIDDLENAME": null,
        "PREFERREDNAME": null,
        "SURNAME": null,
        "EMAILADDRESS": "devi@ruahtech.com.au",
        "EMAILADDRESSALTERNATIVE": null,
        "SEX": null,
        "DOB": null,
        "HISTORICCLIENTID": null,
        "OPTIONALID": null,
        "USI": null,
        "USI_VERIFIED": false,
        "USI_EXEMPTION": false,
        "VSN": null,
        "LUI": null,
        "TFN_RECORDED": false,
        "WORKREADYPARTICIPANTNUMBER": null,
        "SACESTUDENTID": null,
        "POSITION": null,
        "SECTION": null,
        "DIVISION": null,
        "ORGANISATION": null,
        "ORGID": null,
        "ORGIDS": [],
        "BUILDINGNAME": null,
        "UNITNO": null,
        "STREETNO": null,
        "STREETNAME": null,
        "POBOX": null,
        "ADDRESS1": null,
        "ADDRESS2": null,
        "CITY": null,
        "STATE": null,
        "POSTCODE": null,
        "COUNTRYID": null,
        "COUNTRY": null,
        "SBUILDINGNAME": null,
        "SUNITNO": null,
        "SSTREETNO": null,
        "SSTREETNAME": null,
        "SPOBOX": null,
        "SADDRESS1": null,
        "SADDRESS2": null,
        "SCITY": null,
        "SSTATE": null,
        "SPOSTCODE": null,
        "SCOUNTRYID": null,
        "SCOUNTRY": null,
        "TERMADDRESS1": null,
        "TERMADDRESS2": null,
        "TERMCITY": null,
        "TERMSTATE": null,
        "TERMPOSTCODE": null,
        "TERMCOUNTRYID": null,
        "TERMCOUNTRY": null,
        "PHONE": null,
        "MOBILEPHONE": null,
        "WORKPHONE": null,
        "FAX": null,
        "SOURCECODEID": 1,
        "SOURCE": null,
        "COMMENT": null,
        "WEBSITE": null,
        "CITIZENSTATUSID": null,
        "CITIZENSTATUSNAME": null,
        "FKRESIDENCYSTATUSID": null,
        "FKRESIDENCYSTATUSNAME": null,
        "COUNTRYOFBIRTHID": null,
        "COUNTRYOFBIRTHNAME": null,
        "CITYOFBIRTH": null,
        "COUNTRYOFCITIZENID": null,
        "COUNTRYOFCITIZENNAME": null,
        "INDIGENOUSSTATUSID": null,
        "INDIGENOUSSTATUSNAME": null,
        "MAINLANGUAGEID": null,
        "MAINLANGUAGENAME": null,
        "ENGLISHPROFICIENCYID": null,
        "ENGLISHASSISTANCEFLAG": null,
        "HIGHESTSCHOOLLEVELID": null,
        "HIGHESTSCHOOLLEVELYEAR": null,
        "CURRENTSCHOOLLEVEL": null,
        "ATSCHOOLFLAG": null,
        "ATSCHOOLNAME": null,
        "PRIOREDUCATIONIDS": [],
        "PRIOREDUCATIONNAMES": [],
        "PRIOREDUCATIONSTATUS": null,
        "DISABILITYFLAG": null,
        "DISABILITYTYPEIDS": [],
        "DISABILITYTYPENAMES": [],
        "LABOURFORCEID": null,
        "LABOURFORCENAME": null,
        "ANZSCOCODE": null,
        "ANZSICCODE": null,
        "IELTS": null,
        "SURVEYCONTACTSTATUSCODE": null,
        "EMERGENCYCONTACT": null,
        "EMERGENCYCONTACTRELATION": null,
        "EMERGENCYCONTACTPHONE": null,
        "EMPLOYERCONTACTID": null,
        "PAYERCONTACTID": null,
        "SUPERVISORCONTACTID": null,
        "COACHCONTACTID": 12787436,
        "AGENTCONTACTID": null,
        "CONTACTROLEID": null,
        "YEAROFARRIVALAUS": null,
        "CUSTOMFIELD_ADDITIONALSUPPORT": null,
        "CUSTOMFIELD_ADDITIONALSUPPORTDETAILS": null,
        "CUSTOMFIELD_APPRENTICETRAINEE": null,
        "CUSTOMFIELD_APPRENTICESHIP_CENTRE": null,
        "CUSTOMFIELD_APPRENTICESHIP_EMPLOYER": null,
        "CUSTOMFIELD_CONSTRUCTIONEMPLOYED": null,
        "CUSTOMFIELD_COMPLETED_AUSTRALIAN_QUALIFICATIONS_PAST_7_YEARS": null,
        "CUSTOMFIELD_HIGHSCHOOLPREVIOUSQUALINENGLISH": null,
        "CUSTOMFIELD_KNOWLEDGEOFMSANDGOOGLE": null,
        "CUSTOMFIELD_CSQDECLARATION": [],
        "CUSTOMFIELD_COURSEUNITSRELEVANT": null,
        "CUSTOMFIELD_CREDITTRANSFER": null,
        "CUSTOMFIELD_CURRENTJOBROLE": null,
        "CUSTOMFIELD_DEFERRALTASKTRIGGER": null,
        "CUSTOMFIELD_INDUSTRYDUTIES": null,
        "CUSTOMFIELD_DIDYOUCOMPLETETHISQUALIFICATIONINAUSTRALIA": null,
        "CUSTOMFIELD_DIDYOUCOMPLETETHISSCHOOLINGINAUSTRALIA": null,
        "CUSTOMFIELD_SPEAKLANGUAGEOTHERENGLISHATHOME": null,
        "CUSTOMFIELD_EMPLOYER": null,
        "CUSTOMFIELD_EMPLOYMENTSTATUS": null,
        "CUSTOMFIELD_ENGLISHPROFICIENCY": [],
        "CUSTOMFIELD_ENROLMENTPROGRESSTRACKER": null,
        "CUSTOMFIELD_FUNDINGSOURCE": [],
        "CUSTOMFIELD_GHL_ID": null,
        "CUSTOMFIELD_GOALSVISION": null,
        "CUSTOMFIELD_ACCESSTOCOMPUTERANDINTERNET": null,
        "CUSTOMFIELD_PREVIOUSSSFUNDING": null,
        "CUSTOMFIELD_WORKEDINASUPERVISORYMANAGEMENTROLE": null,
        "CUSTOMFIELD_AGREE_TO_THE_INFORMATION_IN_THIS_FORM": null,
        "CUSTOMFIELD_INDUSTRYEXPERIENCE": [],
        "CUSTOMFIELD_INFUSIONSOFTID": null,
        "CUSTOMFIELD_ENGLISHFIRSTLANGUAGE": null,
        "CUSTOMFIELD_NSWHOUSING": null,
        "CUSTOMFIELD_JOBTITLE": null,
        "CUSTOMFIELD_EMPLOYERSERVICE": null,
        "CUSTOMFIELD_LLNREQUIREMENTS": null,
        "CUSTOMFIELD_MOSTRECENTJOBROLE": null,
        "CUSTOMFIELD_SSDECLARATION": [],
        "CUSTOMFIELD_PERSONNOTES": null,
        "CUSTOMFIELD_PREVIOUSLASTNAME": null,
        "CUSTOMFIELD_QUALIFICATION": [],
        "CUSTOMFIELD_SELFPACEDORSCHEDULED": null,
        "CUSTOMFIELD_STUDENTFEE": [],
        "CUSTOMFIELD_STUDENTGOALS": null,
        "CUSTOMFIELD_REWARD1": null,
        "CUSTOMFIELD_REWARD2": null,
        "CUSTOMFIELD_REWARD3": null,
        "CUSTOMFIELD_SUPERVISORYMANAGEMENTROLECOMPANY": null,
        "CUSTOMFIELD_SUPERVISORYMANAGEMENTROLEDETAILS": null,
        "CUSTOMFIELD_SUPERVISORYMANAGEMENTROLENUMBERSUPERVISED": null,
        "CUSTOMFIELD_SUPERVISORYMANAGEMENTROLEREFEREENAME": null,
        "CUSTOMFIELD_SUPERVISORYMANAGEMENTROLEREFEREEPHNUMBER": null,
        "CUSTOMFIELD_SUPERVISORYMANAGEMENTROLEWHENANDHOWLONG": null,
        "CUSTOMFIELD_SUPERVISORYMANAGEMENTROLEYEARSINROLE": null,
        "CUSTOMFIELD_TRAINER1": "Shane Botting",
        "CUSTOMFIELD_TRAINER1NOUNITS": 12,
        "CUSTOMFIELD_TRAINER2": "Shane Botting",
        "CUSTOMFIELD_TRAINER2NOUNITS": 5,
        "CUSTOMFIELD_TRAINER3": null,
        "CUSTOMFIELD_TRAINER3NOUNITS": null,
        "CUSTOMFIELD_VSLDECLARATION": [],
        "CUSTOMFIELD_WAVIER": null,
        "CUSTOMFIELD_WELFARESTATUS": null,
        "CUSTOMFIELD_WELFARETYPE": [],
        "CUSTOMFIELD_YEARSCONTRUCTION": null,
        "CUSTOMFIELD_YEARSOFRELEVANTINDUSTRYEXPERIENCE": null,
        "CUSTOMFIELD_RELEVANTWORKEXPERIENCE": null,
        "CATEGORYIDS": [],
        "LASTUPDATED": "2025-05-15 22:30",
        "CONTACTENTRYDATE": "2024-08-27 14:19",
        "CONTACTACTIVE": true,
        "PHOTO": "//fs.axcelerate.com.au/images/81990022/students/14149898.",
        "DOMAINIDS": []
    }

## LIST STUDENT REGISTERED COURSE

After the student enters the OTP sent to their email address, they are redirected to the dashboard, where a list of their registered courses is displayed.

### URL to get student registered course details

<https://globaltraining.app.axcelerate.com/api/contact/enrolments{contactId}>

### Example Response - Student registered course details

    [
        {
            "ROWID": 1,
            "TYPE": "s",
            "ID": 542904,
            "INSTANCEID": 542904,
            "ENROLID": 14970512,
            "VICENROLMENTID": "3ABAF639-BD2C-4A1C-8B5B-E4EEE0986FAE",
            "INVOICEID": null,
            "INVOICEPAID": false,
            "LEARNERID": 61789683,
            "CODE": "BSBXCM501",
            "LOCATION": "FEE FOR SERVICE NSW 2011",
            "DELIVERY": "Unknown",
            "DELIVERYMODE": "E,W",
            "ACTIVITYTYPE": "Diploma of Business",
            "NAME": "Lead communication in the workplace",
            "COMMENCEDDATE": "2025-01-04",
            "STARTDATE": "2025-01-04",
            "FINISHDATE": "2025-09-04",
            "COMPLETIONDATE": null,
            "MANDATORY": false,
            "STATUS": "NYS",
            "PROGRAMSTATUSIDVIC": null,
            "SCHOOLTYPEID": null,
            "SCHOOLORGID": null,
            "COUNT": 71,
            "OUTCOMECODE": "85"
        },
        {
            "ROWID": 2,
            "TYPE": "s",
            "ID": 542992,
            "INSTANCEID": 542992,
            "ENROLID": 14970512,
            "VICENROLMENTID": "1FC06A71-AC83-45C2-ACB7-C63541C796FF",
            "INVOICEID": null,
            "INVOICEPAID": false,
            "LEARNERID": 61789687,
            "CODE": "BSBWHS521",
            "LOCATION": "FEE FOR SERVICE NSW 2011",
            "DELIVERY": "Unknown",
            "DELIVERYMODE": "E,W",
            "ACTIVITYTYPE": "Diploma of Business",
            "NAME": "Ensure a safe workplace for a work area",
            "COMMENCEDDATE": "2025-05-04",
            "STARTDATE": "2025-05-04",
            "FINISHDATE": "2025-09-04",
            "COMPLETIONDATE": null,
            "MANDATORY": false,
            "STATUS": "NYS",
            "PROGRAMSTATUSIDVIC": null,
            "SCHOOLTYPEID": null,
            "SCHOOLORGID": null,
            "COUNT": 71,
            "OUTCOMECODE": "85"
        },
        {
            "ROWID": 3,
            "TYPE": "s",
            "ID": 542992,
            "INSTANCEID": 542992,
            "ENROLID": 14970515,
            "VICENROLMENTID": "79A37F91-7990-4CB9-9BAA-C26ED8910B01",
            "INVOICEID": null,
            "INVOICEPAID": false,
            "LEARNERID": 61789696,
            "CODE": "BSBWHS521",
            "LOCATION": "FEE FOR SERVICE NSW 2011",
            "DELIVERY": "Unknown",
            "DELIVERYMODE": "E,W",
            "ACTIVITYTYPE": "Diploma of Project Management",
            "NAME": "Ensure a safe workplace for a work area",
            "COMMENCEDDATE": "2026-03-04",
            "STARTDATE": "2026-03-04",
            "FINISHDATE": "2026-03-04",
            "COMPLETIONDATE": null,
            "MANDATORY": false,
            "STATUS": "NYS",
            "PROGRAMSTATUSIDVIC": null,
            "SCHOOLTYPEID": null,
            "SCHOOLORGID": null,
            "COUNT": 71,
            "OUTCOMECODE": "85"
        },
        {
            "ROWID": 4,
            "TYPE": "s",
            "ID": 631769,
            "INSTANCEID": 631769,
            "ENROLID": 14970512,
            "VICENROLMENTID": "6BC4813B-E508-4137-8845-7FB1753DE016",
            "INVOICEID": null,
            "INVOICEPAID": false,
            "LEARNERID": 61789689,
            "CODE": "BSBCRT511",
            "LOCATION": "FEE FOR SERVICE NSW 2011",
            "DELIVERY": "Unknown",
            "DELIVERYMODE": "E,W",
            "ACTIVITYTYPE": "Diploma of Business",
            "NAME": "Develop critical thinking in others",
            "COMMENCEDDATE": "2025-07-04",
            "STARTDATE": "2025-07-04",
            "FINISHDATE": "2025-09-04",
            "COMPLETIONDATE": null,
            "MANDATORY": false,
            "STATUS": "NYS",
            "PROGRAMSTATUSIDVIC": null,
            "SCHOOLTYPEID": null,
            "SCHOOLORGID": null,
            "COUNT": 71,
            "OUTCOMECODE": "85"
        },
        {
            "ROWID": 5,
            "TYPE": "s",
            "ID": 635739,
            "INSTANCEID": 635739,
            "ENROLID": 14970512,
            "VICENROLMENTID": "B90BEB4A-ED57-4E2A-A9CC-76770287732A",
            "INVOICEID": null,
            "INVOICEPAID": false,
            "LEARNERID": 61789688,
            "CODE": "BSBFIN501",
            "LOCATION": "FEE FOR SERVICE NSW 2011",
            "DELIVERY": "Unknown",
            "DELIVERYMODE": "E,W",
            "ACTIVITYTYPE": "Diploma of Business",
            "NAME": "Manage budgets and financial plans",
            "COMMENCEDDATE": "2025-06-04",
            "STARTDATE": "2025-06-04",
            "FINISHDATE": "2025-09-04",
            "COMPLETIONDATE": null,
            "MANDATORY": false,
            "STATUS": "NYS",
            "PROGRAMSTATUSIDVIC": null,
            "SCHOOLTYPEID": null,
            "SCHOOLORGID": null,
            "COUNT": 71,
            "OUTCOMECODE": "85"
        },
        {
            "ROWID": 6,
            "TYPE": "s",
            "ID": 635767,
            "INSTANCEID": 635767,
            "ENROLID": 14970512,
            "VICENROLMENTID": "B700AD2F-6730-47BF-8ED5-1413563BDD1F",
            "INVOICEID": null,
            "INVOICEPAID": false,
            "LEARNERID": 61789685,
            "CODE": "BSBTWK502",
            "LOCATION": "FEE FOR SERVICE NSW 2011",
            "DELIVERY": "Unknown",
            "DELIVERYMODE": "E,W",
            "ACTIVITYTYPE": "Diploma of Business",
            "NAME": "Manage team effectiveness",
            "COMMENCEDDATE": "2025-03-04",
            "STARTDATE": "2025-03-04",
            "FINISHDATE": "2025-09-04",
            "COMPLETIONDATE": null,
            "MANDATORY": false,
            "STATUS": "NYS",
            "PROGRAMSTATUSIDVIC": null,
            "SCHOOLTYPEID": null,
            "SCHOOLORGID": null,
            "COUNT": 71,
            "OUTCOMECODE": "85"
        },
        {
            "ROWID": 7,
            "TYPE": "s",
            "ID": 635767,
            "INSTANCEID": 635767,
            "ENROLID": 14970515,
            "VICENROLMENTID": "9F2C90A1-877B-4BF3-A024-45DF5224BDB1",
            "INVOICEID": null,
            "INVOICEPAID": false,
            "LEARNERID": 61789698,
            "CODE": "BSBTWK502",
            "LOCATION": "FEE FOR SERVICE NSW 2011",
            "DELIVERY": "Unknown",
            "DELIVERYMODE": "E,W",
            "ACTIVITYTYPE": "Diploma of Project Management",
            "NAME": "Manage team effectiveness",
            "COMMENCEDDATE": "2026-03-04",
            "STARTDATE": "2026-03-04",
            "FINISHDATE": "2026-03-04",
            "COMPLETIONDATE": null,
            "MANDATORY": false,
            "STATUS": "NYS",
            "PROGRAMSTATUSIDVIC": null,
            "SCHOOLTYPEID": null,
            "SCHOOLORGID": null,
            "COUNT": 71,
            "OUTCOMECODE": "85"
        },
        {
            "ROWID": 8,
            "TYPE": "s",
            "ID": 635777,
            "INSTANCEID": 635777,
            "ENROLID": 14970512,
            "VICENROLMENTID": "B18C26A0-52DA-494E-8B3F-B7A4160754E2",
            "INVOICEID": null,
            "INVOICEPAID": false,
            "LEARNERID": 61789679,
            "CODE": "BSBPMG530",
            "LOCATION": "FEE FOR SERVICE NSW 2011",
            "DELIVERY": "Unknown",
            "DELIVERYMODE": "E,W",
            "ACTIVITYTYPE": "Diploma of Business",
            "NAME": "Manage project scope",
            "COMMENCEDDATE": "2024-09-04",
            "STARTDATE": "2024-09-04",
            "FINISHDATE": "2025-09-04",
            "COMPLETIONDATE": null,
            "MANDATORY": false,
            "STATUS": "NYS",
            "PROGRAMSTATUSIDVIC": null,
            "SCHOOLTYPEID": null,
            "SCHOOLORGID": null,
            "COUNT": 71,
            "OUTCOMECODE": "85"
        },
        {
            "ROWID": 9,
            "TYPE": "s",
            "ID": 635777,
            "INSTANCEID": 635777,
            "ENROLID": 14970515,
            "VICENROLMENTID": "942A7B03-D21A-4E3B-A2BF-AEF251470D2C",
            "INVOICEID": null,
            "INVOICEPAID": false,
            "LEARNERID": 61789700,
            "CODE": "BSBPMG530",
            "LOCATION": "FEE FOR SERVICE NSW 2011",
            "DELIVERY": "Unknown",
            "DELIVERYMODE": "E,W",
            "ACTIVITYTYPE": "Diploma of Project Management",
            "NAME": "Manage project scope",
            "COMMENCEDDATE": "2026-03-04",
            "STARTDATE": "2026-03-04",
            "FINISHDATE": "2026-03-04",
            "COMPLETIONDATE": null,
            "MANDATORY": false,
            "STATUS": "NYS",
            "PROGRAMSTATUSIDVIC": null,
            "SCHOOLTYPEID": null,
            "SCHOOLORGID": null,
            "COUNT": 71,
            "OUTCOMECODE": "85"
        },
        {
            "ROWID": 10,
            "TYPE": "s",
            "ID": 635778,
            "INSTANCEID": 635778,
            "ENROLID": 14970515,
            "VICENROLMENTID": "681427E9-8FB4-4961-9F10-DB5CDC428EBF",
            "INVOICEID": null,
            "INVOICEPAID": false,
            "LEARNERID": 61789703,
            "CODE": "BSBPMG531",
            "LOCATION": "FEE FOR SERVICE NSW 2011",
            "DELIVERY": "Unknown",
            "DELIVERYMODE": "E,W",
            "ACTIVITYTYPE": "Diploma of Project Management",
            "NAME": "Manage project time",
            "COMMENCEDDATE": "2024-09-04",
            "STARTDATE": "2024-09-04",
            "FINISHDATE": "2026-03-04",
            "COMPLETIONDATE": null,
            "MANDATORY": false,
            "STATUS": "NYS",
            "PROGRAMSTATUSIDVIC": null,
            "SCHOOLTYPEID": null,
            "SCHOOLORGID": null,
            "COUNT": 71,
            "OUTCOMECODE": "85"
        }
    ]

Selected fields are used to construct the course list, along with the corresponding units for each course.
All unit information is mapped to its respective course and organised under that specific course entry.

Course object along with registered units information

    {
        courseId: ENROLID,
        title: ACTIVITYTYPE,
        units: [
            {
                unitId: ID,
                instanceId: INSTANCEID,
                enrolId: ENROLID,
                code: CODE,
                name: NAME,
                status: STATUS
            }
        ]
    }

Upon selecting a course, the associated units within that course are displayed.

Students can then select a unit to either start a chat session or begin an assessment.

## LIST RESOURCES OF A SELECTED UNIT

If the chat option is chosen, the system retrieves the learning resources linked to the selected unit, generates embeddings from those resources, and stores them in the database to enable efficient and contextual responses during the chat.

### URL to get resources based on unit id

<https://globaltraining.app.axcelerate.com/api/course/resources>

 QUERY PARAMS: contactId

### Example Response - Resources available in a unit

    {
        "DIPLOMAS": [],
        "UNITS": [
            {
                "RESOURCES": [
                    {
                        "DOCUMENTNAME": "BSBXCM501 Assessment (PDF)",
                        "CREATEDATE": "2025-01-13 14:46",
                        "DOCUMENTFILENAME": "BSBXCM501 Assessment (PDF) v1.2-20250113044612282.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 453802
                    },
                    {
                        "DOCUMENTNAME": "BSBXCM501 Assessment (WORD)",
                        "CREATEDATE": "2025-01-13 14:46",
                        "DOCUMENTFILENAME": "BSBXCM501 Assessment (WORD) v1.2-20250113044639933.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 453803
                    },
                    {
                        "DOCUMENTNAME": "BSBXCM501 Learner Guide (PDF) v1.2",
                        "CREATEDATE": "2023-07-13 18:07",
                        "DOCUMENTFILENAME": "BSBXCM501-Learner-Guide--PDF-.v1.2.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 430281
                    }
                ],
                "DIPLOMAID": 57079,
                "NAME": "BSBXCM501 - Lead communication in the workplace",
                "ID": 542904
            },
            {
                "RESOURCES": [
                    {
                        "DOCUMENTNAME": "Bogan Building Case Study",
                        "CREATEDATE": "2020-07-22 13:06",
                        "DOCUMENTFILENAME": "Bogan Building Case Study.zip",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 309792
                    },
                    {
                        "DOCUMENTNAME": "BSBWHS521 Assessment (PDF)",
                        "CREATEDATE": "2025-01-13 14:38",
                        "DOCUMENTFILENAME": "BSBWHS521 Assessment (PDF) v1.1-20250113043617714.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 453798
                    },
                    {
                        "DOCUMENTNAME": "BSBWHS521 Assessment (WORD)",
                        "CREATEDATE": "2025-01-13 14:37",
                        "DOCUMENTFILENAME": "BSBWHS521 Assessment (WORD) v1.1-20250113043640766.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 453796
                    },
                    {
                        "DOCUMENTNAME": "BSBWHS521 Construction Safety Additional Info",
                        "CREATEDATE": "2021-01-18 10:34",
                        "DOCUMENTFILENAME": "Construction Safety Additional Info.zip",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 343469
                    },
                    {
                        "DOCUMENTNAME": "BSBWHS521 Learner Guide",
                        "CREATEDATE": "2020-07-22 13:07",
                        "DOCUMENTFILENAME": "BSBWHS521 Learner Guide.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 309796
                    },
                    {
                        "DOCUMENTNAME": "Ensure a safe workplace- GTI PowerPoint",
                        "CREATEDATE": "2020-07-22 13:08",
                        "DOCUMENTFILENAME": "Ensure a safe workplace- GTI Powerpoint CL.pptx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 309798
                    },
                    {
                        "DOCUMENTNAME": "Project Management Case Study",
                        "CREATEDATE": "2020-07-22 13:07",
                        "DOCUMENTFILENAME": "Project Management Case Study.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 309795
                    }
                ],
                "DIPLOMAID": 56973,
                "NAME": "BSBWHS521 - Ensure a safe workplace for a work area",
                "ID": 542992
            },
            {
                "RESOURCES": [
                    {
                        "DOCUMENTNAME": "Bogan Building Case Study",
                        "CREATEDATE": "2020-07-22 13:06",
                        "DOCUMENTFILENAME": "Bogan Building Case Study.zip",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 309792
                    },
                    {
                        "DOCUMENTNAME": "BSBWHS521 Assessment (PDF)",
                        "CREATEDATE": "2025-01-13 14:38",
                        "DOCUMENTFILENAME": "BSBWHS521 Assessment (PDF) v1.1-20250113043617714.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 453798
                    },
                    {
                        "DOCUMENTNAME": "BSBWHS521 Assessment (WORD)",
                        "CREATEDATE": "2025-01-13 14:37",
                        "DOCUMENTFILENAME": "BSBWHS521 Assessment (WORD) v1.1-20250113043640766.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 453796
                    },
                    {
                        "DOCUMENTNAME": "BSBWHS521 Construction Safety Additional Info",
                        "CREATEDATE": "2021-01-18 10:34",
                        "DOCUMENTFILENAME": "Construction Safety Additional Info.zip",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 343469
                    },
                    {
                        "DOCUMENTNAME": "BSBWHS521 Learner Guide",
                        "CREATEDATE": "2020-07-22 13:07",
                        "DOCUMENTFILENAME": "BSBWHS521 Learner Guide.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 309796
                    },
                    {
                        "DOCUMENTNAME": "Ensure a safe workplace- GTI PowerPoint",
                        "CREATEDATE": "2020-07-22 13:08",
                        "DOCUMENTFILENAME": "Ensure a safe workplace- GTI Powerpoint CL.pptx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 309798
                    },
                    {
                        "DOCUMENTNAME": "Project Management Case Study",
                        "CREATEDATE": "2020-07-22 13:07",
                        "DOCUMENTFILENAME": "Project Management Case Study.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 309795
                    }
                ],
                "DIPLOMAID": 57079,
                "NAME": "BSBWHS521 - Ensure a safe workplace for a work area",
                "ID": 542992
            },
            {
                "RESOURCES": [
                    {
                        "DOCUMENTNAME": "BSBCRT511 Additional Learning Resources",
                        "CREATEDATE": "2021-05-31 08:17",
                        "DOCUMENTFILENAME": "BSBCRT511-Additional-Learning-Resources.zip",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 371826
                    },
                    {
                        "DOCUMENTNAME": "BSBCRT511 Assessment (PDF)",
                        "CREATEDATE": "2024-10-08 16:17",
                        "DOCUMENTFILENAME": "BSBCRT511-Assessment--PDF--v1.1.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 450492
                    },
                    {
                        "DOCUMENTNAME": "BSBCRT511 Assessment (WORD)",
                        "CREATEDATE": "2024-10-08 16:17",
                        "DOCUMENTFILENAME": "BSBCRT511-Assessment--WORD--v1.1.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 450493
                    },
                    {
                        "DOCUMENTNAME": "BSBCRT511 Learner Guide",
                        "CREATEDATE": "2023-07-13 17:16",
                        "DOCUMENTFILENAME": "BSBCRT511-Learner-Guide-V1.2.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 430279
                    },
                    {
                        "DOCUMENTNAME": "BSBCRT511 PowerPoint Slides V1.1",
                        "CREATEDATE": "2021-05-31 08:18",
                        "DOCUMENTFILENAME": "BSBCRT511-PowerPoint-Slides-V1.1.pptx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 371828
                    }
                ],
                "DIPLOMAID": 57079,
                "NAME": "BSBCRT511 - Develop critical thinking in others",
                "ID": 631769
            },
            {
                "RESOURCES": [
                    {
                        "DOCUMENTNAME": "BSBFIN501 Assessment (PDF)",
                        "CREATEDATE": "2024-07-31 09:19",
                        "DOCUMENTFILENAME": "BSBFIN501-Assessment--PDF-.v2.3.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 447065
                    },
                    {
                        "DOCUMENTNAME": "BSBFIN501 Assessment (WORD)",
                        "CREATEDATE": "2024-07-31 09:19",
                        "DOCUMENTFILENAME": "BSBFIN501-Assessment--WORD-.v2.3.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 447066
                    },
                    {
                        "DOCUMENTNAME": "BSBFIN501 Budget Task Template",
                        "CREATEDATE": "2023-10-09 08:26",
                        "DOCUMENTFILENAME": "BSBFIN501-Budget-Task-Template-v1.2.xlsx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 433753
                    },
                    {
                        "DOCUMENTNAME": "BSBFIN501 Learner Guide (PDF)",
                        "CREATEDATE": "2024-04-30 14:49",
                        "DOCUMENTFILENAME": "BSBFIN501-Learner-Guide--PDF-.v1.0.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 442843
                    }
                ],
                "DIPLOMAID": 57079,
                "NAME": "BSBFIN501 - Manage budgets and financial plans",
                "ID": 635739
            },
            {
                "RESOURCES": [
                    {
                        "DOCUMENTNAME": "BSBTWK502 Assessment (PDF)",
                        "CREATEDATE": "2024-11-22 15:29",
                        "DOCUMENTFILENAME": "BSBTWK502 Assessment (PDF) v1.4-20241122052904270.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 452340
                    },
                    {
                        "DOCUMENTNAME": "BSBTWK502 Assessment (WORD)",
                        "CREATEDATE": "2024-11-22 15:30",
                        "DOCUMENTFILENAME": "BSBTWK502 Assessment (WORD) v1.4-20241122052957557.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 452341
                    },
                    {
                        "DOCUMENTNAME": "BSBTWK502 Manage team effectiveness Learner guide",
                        "CREATEDATE": "2023-06-28 12:43",
                        "DOCUMENTFILENAME": "BSBTWK502-Manage-team-effectiveness-Learner-guide.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 429171
                    }
                ],
                "DIPLOMAID": 56973,
                "NAME": "BSBTWK502 - Manage team effectiveness",
                "ID": 635767
            },
            {
                "RESOURCES": [
                    {
                        "DOCUMENTNAME": "BSBTWK502 Assessment (PDF)",
                        "CREATEDATE": "2024-11-22 15:29",
                        "DOCUMENTFILENAME": "BSBTWK502 Assessment (PDF) v1.4-20241122052904270.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 452340
                    },
                    {
                        "DOCUMENTNAME": "BSBTWK502 Assessment (WORD)",
                        "CREATEDATE": "2024-11-22 15:30",
                        "DOCUMENTFILENAME": "BSBTWK502 Assessment (WORD) v1.4-20241122052957557.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 452341
                    },
                    {
                        "DOCUMENTNAME": "BSBTWK502 Manage team effectiveness Learner guide",
                        "CREATEDATE": "2023-06-28 12:43",
                        "DOCUMENTFILENAME": "BSBTWK502-Manage-team-effectiveness-Learner-guide.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 429171
                    }
                ],
                "DIPLOMAID": 57079,
                "NAME": "BSBTWK502 - Manage team effectiveness",
                "ID": 635767
            },
            {
                "RESOURCES": [
                    {
                        "DOCUMENTNAME": "BSBPMG530 Assessment (PDF)",
                        "CREATEDATE": "2024-10-23 17:21",
                        "DOCUMENTFILENAME": "BSBPMG530-Assessment--PDF--v1.1.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 451247
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG530 Assessment (Word)",
                        "CREATEDATE": "2024-10-23 17:21",
                        "DOCUMENTFILENAME": "BSBPMG530-Assessment--WORD--v1.1.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 451248
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG530 Case Study 6 & 7 [Construction]",
                        "CREATEDATE": "2024-10-23 17:31",
                        "DOCUMENTFILENAME": "BSBPMG530-Case-Study-6-and-Case-Study-7--Construction--v1.0.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 451250
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG530 CASE STUDY_ Five Coffeeville Project Charters 130821",
                        "CREATEDATE": "2022-01-11 13:23",
                        "DOCUMENTFILENAME": "BSBPMG530-CASE-STUDY_-Five-Coffeeville-Project-Charters-130821.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 405611
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG530 Case_Studies.v1.0",
                        "CREATEDATE": "2022-01-11 13:25",
                        "DOCUMENTFILENAME": "BSBPMG530-Case_Studies.v1.0.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 405612
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG530 Design and construction of the Sydney Opera House",
                        "CREATEDATE": "2022-01-11 13:26",
                        "DOCUMENTFILENAME": "BSBPMG530-Design-and-construction-of-the-Sydney-Opera-House.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 405613
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG530 Learner Guide (PDF)",
                        "CREATEDATE": "2024-03-01 16:14",
                        "DOCUMENTFILENAME": "BSBPMG530-Learner-Guide--PDF-.v1.2.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 440370
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG530 Learner Guide (PowerPoint)",
                        "CREATEDATE": "2021-10-13 15:59",
                        "DOCUMENTFILENAME": "BSBPMG530-Learner-Guide--PowerPoint-.pptx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 404106
                    }
                ],
                "DIPLOMAID": 56973,
                "NAME": "BSBPMG530 - Manage project scope",
                "ID": 635777
            },
            {
                "RESOURCES": [
                    {
                        "DOCUMENTNAME": "BSBPMG530 Assessment (PDF)",
                        "CREATEDATE": "2024-10-23 17:21",
                        "DOCUMENTFILENAME": "BSBPMG530-Assessment--PDF--v1.1.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 451247
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG530 Assessment (Word)",
                        "CREATEDATE": "2024-10-23 17:21",
                        "DOCUMENTFILENAME": "BSBPMG530-Assessment--WORD--v1.1.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 451248
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG530 Case Study 6 & 7 [Construction]",
                        "CREATEDATE": "2024-10-23 17:31",
                        "DOCUMENTFILENAME": "BSBPMG530-Case-Study-6-and-Case-Study-7--Construction--v1.0.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 451250
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG530 CASE STUDY_ Five Coffeeville Project Charters 130821",
                        "CREATEDATE": "2022-01-11 13:23",
                        "DOCUMENTFILENAME": "BSBPMG530-CASE-STUDY_-Five-Coffeeville-Project-Charters-130821.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 405611
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG530 Case_Studies.v1.0",
                        "CREATEDATE": "2022-01-11 13:25",
                        "DOCUMENTFILENAME": "BSBPMG530-Case_Studies.v1.0.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 405612
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG530 Design and construction of the Sydney Opera House",
                        "CREATEDATE": "2022-01-11 13:26",
                        "DOCUMENTFILENAME": "BSBPMG530-Design-and-construction-of-the-Sydney-Opera-House.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 405613
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG530 Learner Guide (PDF)",
                        "CREATEDATE": "2024-03-01 16:14",
                        "DOCUMENTFILENAME": "BSBPMG530-Learner-Guide--PDF-.v1.2.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 440370
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG530 Learner Guide (PowerPoint)",
                        "CREATEDATE": "2021-10-13 15:59",
                        "DOCUMENTFILENAME": "BSBPMG530-Learner-Guide--PowerPoint-.pptx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 404106
                    }
                ],
                "DIPLOMAID": 57079,
                "NAME": "BSBPMG530 - Manage project scope",
                "ID": 635777
            },
            {
                "RESOURCES": [
                    {
                        "DOCUMENTNAME": "Agile Gantt Chart Template",
                        "CREATEDATE": "2021-10-07 17:01",
                        "DOCUMENTFILENAME": "Agile-Gantt-Chart-Template.xlsx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 404048
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG531 Assessment (PDF)",
                        "CREATEDATE": "2024-10-28 13:29",
                        "DOCUMENTFILENAME": "BSBPMG531-Assessment--PDF--v1.2.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 451377
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG531 Assessment (WORD)",
                        "CREATEDATE": "2024-10-28 13:29",
                        "DOCUMENTFILENAME": "BSBPMG531-Assessment--WORD--v1.2.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 451378
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG531 Learner Guide (PDF)",
                        "CREATEDATE": "2024-07-09 08:17",
                        "DOCUMENTFILENAME": "BSBPMG531-Learner-Guide--PDF-.v1.0.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 445774
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG531 Learner Guide PowerPoint",
                        "CREATEDATE": "2021-10-07 17:01",
                        "DOCUMENTFILENAME": "BSBPMG531-Learner-Guide-PowerPoint.pptx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 404050
                    },
                    {
                        "DOCUMENTNAME": "Coffeville Project Charter examples",
                        "CREATEDATE": "2022-03-07 16:12",
                        "DOCUMENTFILENAME": "CASE-STUDY_-Five-Coffeeville-Project-Charters-130821.v1.0.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 407370
                    },
                    {
                        "DOCUMENTNAME": "Vertex42 Excel Gantt Chart Template",
                        "CREATEDATE": "2021-10-07 17:02",
                        "DOCUMENTFILENAME": "Vertex42-Excel-Gantt-Chart-Template.xlsx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 404051
                    }
                ],
                "DIPLOMAID": 56973,
                "NAME": "BSBPMG531 - Manage project time",
                "ID": 635778
            },
            {
                "RESOURCES": [
                    {
                        "DOCUMENTNAME": "BSBPMG532 Assessment (PDF)",
                        "CREATEDATE": "2024-11-01 16:20",
                        "DOCUMENTFILENAME": "BSBPMG532-Assessment--PDF--v1.2.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 451634
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG532 Assessment (WORD)",
                        "CREATEDATE": "2024-11-01 16:20",
                        "DOCUMENTFILENAME": "BSBPMG532-Assessment--WORD--v1.2.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 451635
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG532 Learner Guide",
                        "CREATEDATE": "2023-08-07 10:37",
                        "DOCUMENTFILENAME": "BSBPMG532-Learner-Guide.v1.1.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 431221
                    }
                ],
                "DIPLOMAID": 56973,
                "NAME": "BSBPMG532 - Manage project quality",
                "ID": 635779
            },
            {
                "RESOURCES": [
                    {
                        "DOCUMENTNAME": "BSBPMG533 Assessment (PDF)",
                        "CREATEDATE": "2024-11-15 14:07",
                        "DOCUMENTFILENAME": "BSBPMG533 Assessment (PDF) v1.3-20241115040701773.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 452037
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG533 Assessment (WORD)",
                        "CREATEDATE": "2024-11-15 14:07",
                        "DOCUMENTFILENAME": "BSBPMG533 Assessment (WORD) v1.3-20241115040715461.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 452038
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG533 Learner Guide - (Powerpoint)",
                        "CREATEDATE": "2021-09-16 16:41",
                        "DOCUMENTFILENAME": "BSBPMG533-Learner-Guide----Powerpoint-.pptx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 401411
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG533 Learner Guide (PDF)",
                        "CREATEDATE": "2023-08-07 11:32",
                        "DOCUMENTFILENAME": "BSBPMG533-Learner-Guide--PDF-.v1.2.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 431225
                    },
                    {
                        "DOCUMENTNAME": "T2201.3 Project-Budget Template",
                        "CREATEDATE": "2021-09-16 16:43",
                        "DOCUMENTFILENAME": "T2201.3-Project-Budget-Template.xlsx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 401416
                    }
                ],
                "DIPLOMAID": 56973,
                "NAME": "BSBPMG533 - Manage project cost",
                "ID": 635780
            },
            {
                "RESOURCES": [
                    {
                        "DOCUMENTNAME": "BSBPMG534 Assessment (PDF)",
                        "CREATEDATE": "2024-11-01 16:27",
                        "DOCUMENTFILENAME": "BSBPMG534-Assessment--PDF--v1.1.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 451637
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG534 Assessment (WORD)",
                        "CREATEDATE": "2024-11-01 16:27",
                        "DOCUMENTFILENAME": "BSBPMG534-Assessment--WORD--v1.1.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 451638
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG534 Learner Guide (PDF)",
                        "CREATEDATE": "2024-07-09 10:55",
                        "DOCUMENTFILENAME": "BSBPMG534-Learner-Guide--PDF-.v1.0.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 445815
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG534 Manage Project Human Resources PowerPoint",
                        "CREATEDATE": "2021-12-07 11:20",
                        "DOCUMENTFILENAME": "BSBPMG534-Manage-Project-Human-Resources-PowerPoint.pptx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 405025
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG534 Performance improvement plan - Template",
                        "CREATEDATE": "2021-12-07 11:22",
                        "DOCUMENTFILENAME": "BSBPMG534-Performance-improvement-plan---Template.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 405026
                    }
                ],
                "DIPLOMAID": 56973,
                "NAME": "BSBPMG534 - Manage project human resources",
                "ID": 635781
            },
            {
                "RESOURCES": [
                    {
                        "DOCUMENTNAME": "BSBPMG534 Assessment (PDF)",
                        "CREATEDATE": "2024-11-01 16:27",
                        "DOCUMENTFILENAME": "BSBPMG534-Assessment--PDF--v1.1.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 451637
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG534 Assessment (WORD)",
                        "CREATEDATE": "2024-11-01 16:27",
                        "DOCUMENTFILENAME": "BSBPMG534-Assessment--WORD--v1.1.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 451638
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG534 Learner Guide (PDF)",
                        "CREATEDATE": "2024-07-09 10:55",
                        "DOCUMENTFILENAME": "BSBPMG534-Learner-Guide--PDF-.v1.0.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 445815
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG534 Manage Project Human Resources PowerPoint",
                        "CREATEDATE": "2021-12-07 11:20",
                        "DOCUMENTFILENAME": "BSBPMG534-Manage-Project-Human-Resources-PowerPoint.pptx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 405025
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG534 Performance improvement plan - Template",
                        "CREATEDATE": "2021-12-07 11:22",
                        "DOCUMENTFILENAME": "BSBPMG534-Performance-improvement-plan---Template.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 405026
                    }
                ],
                "DIPLOMAID": 57079,
                "NAME": "BSBPMG534 - Manage project human resources",
                "ID": 635781
            },
            {
                "RESOURCES": [
                    {
                        "DOCUMENTNAME": "BSBPMG535 Assessment (PDF)",
                        "CREATEDATE": "2024-11-01 16:46",
                        "DOCUMENTFILENAME": "BSBPMG535-Assessment--PDF--v1.1.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 451640
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG535 Assessment (WORD)",
                        "CREATEDATE": "2024-11-01 16:46",
                        "DOCUMENTFILENAME": "BSBPMG535-Assessment--WORD--v1.1.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 451641
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG535 Learner Guide (PDF)",
                        "CREATEDATE": "2023-08-07 13:34",
                        "DOCUMENTFILENAME": "BSBPMG535-Learner-Guide--PDF-.v1.1.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 431240
                    }
                ],
                "DIPLOMAID": 56973,
                "NAME": "BSBPMG535 - Manage project information and communication",
                "ID": 635782
            },
            {
                "RESOURCES": [
                    {
                        "DOCUMENTNAME": "BSBPMG535 Assessment (PDF)",
                        "CREATEDATE": "2024-11-01 16:46",
                        "DOCUMENTFILENAME": "BSBPMG535-Assessment--PDF--v1.1.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 451640
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG535 Assessment (WORD)",
                        "CREATEDATE": "2024-11-01 16:46",
                        "DOCUMENTFILENAME": "BSBPMG535-Assessment--WORD--v1.1.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 451641
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG535 Learner Guide (PDF)",
                        "CREATEDATE": "2023-08-07 13:34",
                        "DOCUMENTFILENAME": "BSBPMG535-Learner-Guide--PDF-.v1.1.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 431240
                    }
                ],
                "DIPLOMAID": 57079,
                "NAME": "BSBPMG535 - Manage project information and communication",
                "ID": 635782
            },
            {
                "RESOURCES": [
                    {
                        "DOCUMENTNAME": "BSBPMG536 Assessment (PDF)",
                        "CREATEDATE": "2024-11-22 14:53",
                        "DOCUMENTFILENAME": "BSBPMG536 Assessment (PDF) v2.0-20241122045239307.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 452327
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG536 Assessment (WORD)",
                        "CREATEDATE": "2024-11-22 14:53",
                        "DOCUMENTFILENAME": "BSBPMG536 Assessment (WORD) v2.0-20241122045336331.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 452328
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG536 Learner Guide (PDF)",
                        "CREATEDATE": "2024-07-09 13:13",
                        "DOCUMENTFILENAME": "BSBPMG536-Learner-Guide--PDF-.v1.0.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 445840
                    },
                    {
                        "DOCUMENTNAME": "CoffeeVille-Risk-Management-Strategy-and-Plan",
                        "CREATEDATE": "2021-10-08 17:05",
                        "DOCUMENTFILENAME": "CoffeeVille-Risk-Management-Strategy-and-Plan.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 404080
                    },
                    {
                        "DOCUMENTNAME": "IRM-Report-ISO-31000-2018-v3",
                        "CREATEDATE": "2023-03-28 12:24",
                        "DOCUMENTFILENAME": "IRM-Report-ISO-31000-2018-v3.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 425863
                    },
                    {
                        "DOCUMENTNAME": "ISO_31000_2018",
                        "CREATEDATE": "2023-03-28 12:26",
                        "DOCUMENTFILENAME": "ISO_31000_2018-1-.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 425864
                    },
                    {
                        "DOCUMENTNAME": "Risk Register Template (EXCEL)",
                        "CREATEDATE": "2023-04-04 16:23",
                        "DOCUMENTFILENAME": "Excel-Risk-Register-Template.xlsx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 426169
                    }
                ],
                "DIPLOMAID": 56973,
                "NAME": "BSBPMG536 - Manage project risk",
                "ID": 635783
            },
            {
                "RESOURCES": [
                    {
                        "DOCUMENTNAME": "BSBPMG540 Assessment (PDF)",
                        "CREATEDATE": "2024-11-01 16:49",
                        "DOCUMENTFILENAME": "BSBPMG540-Assessment--PDF--v1.1.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 451643
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG540 Assessment (WORD)",
                        "CREATEDATE": "2024-11-01 16:49",
                        "DOCUMENTFILENAME": "BSBPMG540-Assessment--WORD--v1.1.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 451644
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG540 Learner Guide",
                        "CREATEDATE": "2023-11-08 14:17",
                        "DOCUMENTFILENAME": "BSBPMG540-Learner-Guide.v1.0.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 435044
                    },
                    {
                        "DOCUMENTNAME": "BSBPMG540 Template",
                        "CREATEDATE": "2024-11-01 16:49",
                        "DOCUMENTFILENAME": "BSBPMG540-Template.v1.1.doc",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 451646
                    }
                ],
                "DIPLOMAID": 56973,
                "NAME": "BSBPMG540 - Manage project integration",
                "ID": 635784
            },
            {
                "RESOURCES": [
                    {
                        "DOCUMENTNAME": "BSBTWK503 Assessment (PDF)",
                        "CREATEDATE": "2024-10-08 14:37",
                        "DOCUMENTFILENAME": "BSBTWK503-Assessment--PDF--v1.5.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 450477
                    },
                    {
                        "DOCUMENTNAME": "BSBTWK503 Assessment (WORD)",
                        "CREATEDATE": "2024-10-08 14:37",
                        "DOCUMENTFILENAME": "BSBTWK503-Assessment--WORD--v1.5.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 450478
                    },
                    {
                        "DOCUMENTNAME": "BSBTWK503 Case Study",
                        "CREATEDATE": "2021-08-06 16:26",
                        "DOCUMENTFILENAME": "BSBTWK503-Case-Study.zip",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 388726
                    },
                    {
                        "DOCUMENTNAME": "BSBTWK503 Learner Guide (PDF)",
                        "CREATEDATE": "2024-07-11 13:07",
                        "DOCUMENTFILENAME": "BSBTWK503-Learner-Guide--PDF-.v1.1.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 446020
                    },
                    {
                        "DOCUMENTNAME": "BSBTWK503 Optional Assessment Templates",
                        "CREATEDATE": "2020-07-07 16:25",
                        "DOCUMENTFILENAME": "Templates avalible for use..zip",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 307339
                    }
                ],
                "DIPLOMAID": 56973,
                "NAME": "BSBTWK503 - Manage meetings",
                "ID": 636243
            },
            {
                "RESOURCES": [
                    {
                        "DOCUMENTNAME": "BSBTWK503 Assessment (PDF)",
                        "CREATEDATE": "2024-10-08 14:37",
                        "DOCUMENTFILENAME": "BSBTWK503-Assessment--PDF--v1.5.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 450477
                    },
                    {
                        "DOCUMENTNAME": "BSBTWK503 Assessment (WORD)",
                        "CREATEDATE": "2024-10-08 14:37",
                        "DOCUMENTFILENAME": "BSBTWK503-Assessment--WORD--v1.5.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 450478
                    },
                    {
                        "DOCUMENTNAME": "BSBTWK503 Case Study",
                        "CREATEDATE": "2021-08-06 16:26",
                        "DOCUMENTFILENAME": "BSBTWK503-Case-Study.zip",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 388726
                    },
                    {
                        "DOCUMENTNAME": "BSBTWK503 Learner Guide (PDF)",
                        "CREATEDATE": "2024-07-11 13:07",
                        "DOCUMENTFILENAME": "BSBTWK503-Learner-Guide--PDF-.v1.1.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 446020
                    },
                    {
                        "DOCUMENTNAME": "BSBTWK503 Optional Assessment Templates",
                        "CREATEDATE": "2020-07-07 16:25",
                        "DOCUMENTFILENAME": "Templates avalible for use..zip",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 307339
                    }
                ],
                "DIPLOMAID": 57079,
                "NAME": "BSBTWK503 - Manage meetings",
                "ID": 636243
            },
            {
                "RESOURCES": [
                    {
                        "DOCUMENTNAME": "BSBOPS504 Assessment (PDF)",
                        "CREATEDATE": "2024-11-13 15:00",
                        "DOCUMENTFILENAME": "BSBOPS504-Assessment--PDF--v1.5.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 451966
                    },
                    {
                        "DOCUMENTNAME": "BSBOPS504 Assessment (WORD)",
                        "CREATEDATE": "2024-11-13 15:01",
                        "DOCUMENTFILENAME": "BSBOPS504-Assessment--Word-.v1.4.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 451969
                    },
                    {
                        "DOCUMENTNAME": "BSBOPS504 Learner Guide (PDF)",
                        "CREATEDATE": "2023-07-31 16:00",
                        "DOCUMENTFILENAME": "BSBOPS504-Learner-Guide--PDF-.v1.2.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 431026
                    },
                    {
                        "DOCUMENTNAME": "IRM-Report-ISO-31000-2018-v3",
                        "CREATEDATE": "2023-03-28 12:24",
                        "DOCUMENTFILENAME": "IRM-Report-ISO-31000-2018-v3.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 425863
                    },
                    {
                        "DOCUMENTNAME": "ISO_31000_2018",
                        "CREATEDATE": "2023-03-28 12:26",
                        "DOCUMENTFILENAME": "ISO_31000_2018-1-.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 425864
                    }
                ],
                "DIPLOMAID": 56973,
                "NAME": "BSBOPS504 - Manage business risk",
                "ID": 636244
            },
            {
                "RESOURCES": [
                    {
                        "DOCUMENTNAME": "BSBOPS504 Assessment (PDF)",
                        "CREATEDATE": "2024-11-13 15:00",
                        "DOCUMENTFILENAME": "BSBOPS504-Assessment--PDF--v1.5.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 451966
                    },
                    {
                        "DOCUMENTNAME": "BSBOPS504 Assessment (WORD)",
                        "CREATEDATE": "2024-11-13 15:01",
                        "DOCUMENTFILENAME": "BSBOPS504-Assessment--Word-.v1.4.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 451969
                    },
                    {
                        "DOCUMENTNAME": "BSBOPS504 Learner Guide (PDF)",
                        "CREATEDATE": "2023-07-31 16:00",
                        "DOCUMENTFILENAME": "BSBOPS504-Learner-Guide--PDF-.v1.2.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 431026
                    },
                    {
                        "DOCUMENTNAME": "IRM-Report-ISO-31000-2018-v3",
                        "CREATEDATE": "2023-03-28 12:24",
                        "DOCUMENTFILENAME": "IRM-Report-ISO-31000-2018-v3.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 425863
                    },
                    {
                        "DOCUMENTNAME": "ISO_31000_2018",
                        "CREATEDATE": "2023-03-28 12:26",
                        "DOCUMENTFILENAME": "ISO_31000_2018-1-.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 425864
                    }
                ],
                "DIPLOMAID": 57079,
                "NAME": "BSBOPS504 - Manage business risk",
                "ID": 636244
            },
            {
                "RESOURCES": [
                    {
                        "DOCUMENTNAME": "BSBOPS501 Assessment (PDF)",
                        "CREATEDATE": "2024-11-08 11:36",
                        "DOCUMENTFILENAME": "BSBOPS501-Assessment--PDF--v1.5.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 451812
                    },
                    {
                        "DOCUMENTNAME": "BSBOPS501 Assessment (WORD)",
                        "CREATEDATE": "2024-11-08 11:36",
                        "DOCUMENTFILENAME": "BSBOPS501-Assessment--WORD--v1.5.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 451813
                    },
                    {
                        "DOCUMENTNAME": "BSBOPS501 Learner Guide",
                        "CREATEDATE": "2024-06-13 15:14",
                        "DOCUMENTFILENAME": "BSBOPS501-Learner-Guide.v1.0.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 444918
                    },
                    {
                        "DOCUMENTNAME": "BSBOPS501 Resource Plan Template",
                        "CREATEDATE": "2022-08-18 12:27",
                        "DOCUMENTFILENAME": "BSBOPS501-Resource-Plan-Template.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 414957
                    }
                ],
                "DIPLOMAID": 57079,
                "NAME": "BSBOPS501 - Manage business resources",
                "ID": 636246
            },
            {
                "RESOURCES": [
                    {
                        "DOCUMENTNAME": "BSBSUS511 Assessment (PDF)",
                        "CREATEDATE": "2021-11-11 11:59",
                        "DOCUMENTFILENAME": "BSBSUS511-Assessment--PDF-.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 404593
                    },
                    {
                        "DOCUMENTNAME": "BSBSUS511 Assessment (PDF)",
                        "CREATEDATE": "2024-11-08 11:28",
                        "DOCUMENTFILENAME": "BSBSUS511-Assessment--PDF--v1.2.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 451806
                    },
                    {
                        "DOCUMENTNAME": "BSBSUS511 Assessment (WORD)",
                        "CREATEDATE": "2021-11-11 11:58",
                        "DOCUMENTFILENAME": "BSBSUS511-Assessment--WORD-.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 404592
                    },
                    {
                        "DOCUMENTNAME": "BSBSUS511 Assessment (WORD)",
                        "CREATEDATE": "2024-11-08 11:28",
                        "DOCUMENTFILENAME": "BSBSUS511-Assessment--WORD--v1.2.docx",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 451807
                    },
                    {
                        "DOCUMENTNAME": "BSBSUS511 Learners Guide",
                        "CREATEDATE": "2024-04-17 15:12",
                        "DOCUMENTFILENAME": "BSBSUS511-Learners-Guide.v1.0.pdf",
                        "INTEGRATIONID": "",
                        "CATEGORY": "",
                        "DOCUMENTID": 442483
                    }
                ],
                "DIPLOMAID": 57079,
                "NAME": "BSBSUS511 - Develop workplace policies and procedures for sustainability",
                "ID": 636248
            }
        ],
        "WORKSHOPS": [],
        "POLICIESFORMS": {
            "POLICIES": {
                "Newsletters": [
                    {
                        "DOCUMENTNAME": "GTI News",
                        "DOCUMENTFILENAME": "GTI-News---July-2024.pdf",
                        "SUBGROUP": "",
                        "DOCUMENTID": 447108
                    }
                ]
            },
            "FORMS": {
                "Completions": [
                    {
                        "DOCUMENTNAME": "Completed Qualification Request Form",
                        "DOCUMENTFILENAME": "https://globaltraining.edu.au/global_training_institute/forms/form-application-final-documents/",
                        "SUBGROUP": "",
                        "DOCUMENTID": 306971
                    },
                    {
                        "DOCUMENTNAME": "Student Surveys",
                        "DOCUMENTFILENAME": "https://globaltraining.edu.au/global_training_institute/student-surveys/",
                        "SUBGROUP": "",
                        "DOCUMENTID": 306981
                    },
                    {
                        "DOCUMENTNAME": "Training Plan Completion Signature",
                        "DOCUMENTFILENAME": "https://globaltraining.edu.au/global_training_institute/training-plan-completion-signature/",
                        "SUBGROUP": "",
                        "DOCUMENTID": 306983
                    }
                ],
                "General": [
                    {
                        "DOCUMENTNAME": "Complaints, Grievances & Appeals",
                        "DOCUMENTFILENAME": "https://globaltraining.edu.au/global_training_institute/forms/complaints-grievances-appeals/",
                        "SUBGROUP": "",
                        "DOCUMENTID": 306989
                    },
                    {
                        "DOCUMENTNAME": "Confirmation of Enrolment, or Statement of Results Request Form",
                        "DOCUMENTFILENAME": "https://globaltraining.edu.au/global_training_institute/forms/form-confirmation-enrolment-statement-results-request/",
                        "SUBGROUP": "",
                        "DOCUMENTID": 306991
                    },
                    {
                        "DOCUMENTNAME": "Early Trimester Completion Form",
                        "DOCUMENTFILENAME": "https://globaltraining.edu.au/global_training_institute/early-completion-form-trimester/",
                        "SUBGROUP": "",
                        "DOCUMENTID": 306987
                    },
                    {
                        "DOCUMENTNAME": "Incident Form",
                        "DOCUMENTFILENAME": "https://globaltraining.edu.au/global_training_institute/forms/form-incident-form/",
                        "SUBGROUP": "",
                        "DOCUMENTID": 306990
                    },
                    {
                        "DOCUMENTNAME": "Notification of Withdrawal from Course",
                        "DOCUMENTFILENAME": "https://globaltraining.edu.au/global_training_institute/forms/form-notification-withdrawal/",
                        "SUBGROUP": "",
                        "DOCUMENTID": 306992
                    },
                    {
                        "DOCUMENTNAME": "Request for Course Extension",
                        "DOCUMENTFILENAME": "https://globaltraining.edu.au/global_training_institute/forms/form-request-extension/",
                        "SUBGROUP": "",
                        "DOCUMENTID": 306994
                    },
                    {
                        "DOCUMENTNAME": "Request for Deferral or Suspension",
                        "DOCUMENTFILENAME": "https://globaltraining.edu.au/global_training_institute/forms/form-request-deferal-suspension/",
                        "SUBGROUP": "",
                        "DOCUMENTID": 306993
                    },
                    {
                        "DOCUMENTNAME": "Request for Reissuing Certificate/Qualification",
                        "DOCUMENTFILENAME": "https://globaltraining.edu.au/global_training_institute/forms/form-request-reissuing-certificatequalification/",
                        "SUBGROUP": "",
                        "DOCUMENTID": 306995
                    },
                    {
                        "DOCUMENTNAME": "Training Plan Beginning Signature",
                        "DOCUMENTFILENAME": "https://globaltraining.edu.au/global_training_institute/training-plan-beginning-signature-nsw-ss/",
                        "SUBGROUP": "",
                        "DOCUMENTID": 306985
                    },
                    {
                        "DOCUMENTNAME": "Update Contact Details",
                        "DOCUMENTFILENAME": "https://globaltraining.edu.au/global_training_institute/forms/form-update-contact-details/",
                        "SUBGROUP": "",
                        "DOCUMENTID": 306988
                    }
                ]
            }
        },
        "TRAININGRELATED": [
            {
                "DOCUMENTNAME": "BSBTWK502 Assessment (WORD)",
                "CREATEDATE": "2023-06-27 09:58",
                "DOCUMENTFILENAME": "BSBTWK502-Assessment--WORD-.v1.1-2-(C5E5C375-C036-44E4-A2F6-17B3DD74AAC3).docx",
                "INTEGRATIONID": "",
                "CATEGORY": "",
                "DOCUMENTID": 429080
            },
            {
                "DOCUMENTNAME": "GTI Resource Library",
                "CREATEDATE": "2020-11-24 17:44",
                "DOCUMENTFILENAME": "https://globaltraining.edu.au/global_training_institute/resource-library/",
                "INTEGRATIONID": "",
                "CATEGORY": "",
                "DOCUMENTID": 335755
            }
        ]
    }

Based on the provided data, a specific unit is identified by matching its ID within the UNITS array. Once the relevant unit object is retrieved, its RESOURCES array is accessed and processes only the supported file types—namely, PDF (.pdf), Microsoft Word (.doc), and Word Open XML (.docx)—for embedding purposes.

Once the embedding process is completed, the document ID of the resource is stored in a separate collection within the database, along with an embedding status marked as completed. When a student selects the chat option for a unit, the system first checks this collection to determine whether the resource with the corresponding document ID has already been embedded. If the embedding is marked as completed, the system skips reembedding that resource.

After the embedding process is complete, the student can initiate a chat with the AI for the selected unit.

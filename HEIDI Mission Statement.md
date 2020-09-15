Higher Education Interoperable Data Initiative (HEIDI)
======================================================

Introduction and Goals
----------------------

There are a number of data-related projects and systems in European higher education, tackling student data, statistics or databases of institutions, amongst others. At the moment, we are not really interoperable. This creates costs, ineffeciencies and lack of transparency. In their draft Rome Communiqué[[1]](#f1), to be adopted in November 2020, European ministers of higher education recognise the need "to enhance the interoperability of digital systems and the exchange of student and institutional data, in full respect of privacy and security".

We would thus like to see these projects/systems interoperate seamlessly and thus serve best a large number of users in the European higher education community. Better linking the various data sets and systems would maximise their potential, transferring or correlating data between different systems may open entirely new use cases or valuable insights.

A range of informal conversations were held on the need to address interoperability between a range of individuals and initiatives throughout 2019, including the European University Foundation (EUF), the European Quality Assurance Register (EQAR) and the Europass Interoperability Expert. These have worked together to prepare for a first meeting.

In its [DEQAR CONNECT project](https://www.eqar.eu/kb/projects/deqar-connect/), EQAR undertook to convene a roundtable of higher education data-related projects and initiatives, and to initiate a discussion on interoperability. EQAR therefore volunteers to host an initial meeting as part of the DEQAR CONNECT project, but considers that HEIDI should then develop into a self-standing initiative.

Overview of Problem Domains
---------------------------

There are various problem domains, some more pressing than others. The following inventory is in order of priority:

### Identifiers

Identifiers are needed to unambiguously identify entities when communicating or transfering data between systems. The following entities frequently need to be identified in higher education:

1. Countries and higher education systems
1. Higher education institutions
1. Study programmes
1. Courses or modules
1. Students

For countries, ISO codes are established identifiers.

Higher education institutions are a pivotal enitity, and institutional identifiers thus a matter of priority. Various approaches already exist (e.g. PIC, ETER, Erasmus Code, EIDAS), but are not articulated to each other. At the same time, given less than 10000 HEIs in Europe the numbers are relatively managable.

For study programmes, courses and students numbers are larger by magnitudes.

For students, a European Student ID is under development as a federated/delegated system based on institutional student IDs.

### Data Structure

Different systems should use agreed data models/structures, or at least make the data models/structures they use fully transparent. This will allow easy communication and conversion of data between systems. An agreement would cover the minimum fields different data models should harmonise, for the purposes of promoting interoperability.

Different organisations, dealing with such data, have already developed their data models. These should be used as a starting point.

### Data Availability

Data on students and their achievement is personal data and will thus generally be private.

All other data discussed herein (institutions, courses, etc.) is inherently public. In addition to being accessible through a public web interface, all projects/systems should also make their data fully open and accessible for download or through an API.

### Data Portability

*(placeholder)*

### Other Issues

*(placeholder)*

Initiatives Requiring Interoperability
--------------------------------------

There are numerous local, regional, national, European and international initiatives that deal with data in higher education. HEIDI aims to bring together the essential European-level projects and systems, focusing on publicly-funded or publicly-endorsed ones with systemic impact on a European scale.

The following initiatives are invited to the initial roundtable:

- Europass Digital Credentials Infrastructure (EDCI)
- Erasmus Without Paper (EWP)
- Emrex (implementing ELMO spec)
- European Student Card (ESC)
- Erasmus+ App
- My Academic ID
- Database of External Quality Assurance Results (DEQAR)
- European Tertiary Education Register (ETER)
- DiploMe
- IAU World Higher Education Database (WHED)

Additional initiatives might join HEIDI in agreement with those already involved.

Design Requirements for an Interoperability Initiative
------------------------------------------------------

Given the rapid progress of these initiatives and the policy priority attached to digitalisation, the Initiative needs to be able to act and reach agreement on crucial standards quickly.

### Scope

It is suggested that the Initiative focuses on higher education within the 48 countries making up the European Higher Education Area (EHEA). (Nevertheless, results might be scalable geographically or transferable to other sectors later on.)

### Governance Requirements

The Initiative should be stakeholder-led, that is, driven by the initiatives concerned. The organisations running these initiatives have expertise in their field and are best-placed to agree on standards jointly.

It should be ensured that the European Commission, governments and further stakeholders (e.g. European representative organisations) endorse the Initiative's efforts and standards. Given the scope, this could be best achieved by informing the EHEA's working structures, i.e. the Bologna Follow-Up Group (BFUG), and possibly suggesting that the Initiative become part of the 2020-2023 EHEA work programme.

The Initiative recognises that different organisations each manage specific initiatives/systems within their own remit, and does not aim to change these.

### Licence Requirements
Free (as in air)

Working Methods
---------------

Any group of members of the group may propose a problem domain to be addressed. Prioritisation of problem domains are the remit of the whole group.

Each problem domain should be tackled via regular web conferences, held at least once a month. 

Typically a problem domain should be managed by a *policy group* supported by a *technical group* who gives independent technical advice to the policy group.

Each problem domain must follow a standardised procedure for resolution:

1.  **Definition of Use Cases**

    Definition of use cases is the first step. It involves member organisations explaining the issues they wish to solve under the problem domain. Use cases must be accepted by the group working on the domain for inclusion. A procedure is outlined [here](Supporting/UseCaseTemplate.md). Use cases should ideally be defined by persons who work with them.

2.  **Proposal of Requirements**

    Based on the use cases a proposal for requirements for a technical solution will be prepared. The requirements set the minimum criteria the solution must meet to be considered acceptable. Requirements should be made on the proposal of technical experts, and endorsed by the wider policy group.

3.  **Outline of Scenarios for Technical Solutions**

    It is the mandate of the technical group to propose a menu of technical scenarios which match the requirements. The following provides high-level guidance on possible [architectural scenarios](Supporting/Architectural%20Scenarios.md).

4.  **Selection of a Preferred Implementation Scenario**

    The policy group will discuss, improve and select a preferred implementation scenario from the options presented.

5.  **Publication of Standard**

    The decision of the policy group will then be translated into a documented agreement covering policy, governance, content and  technical aspects, to be authored jointly by the policy and technical groups.

6.  **Agreement of  Standard**

    Once the standard is published, members/organisations should notify their implementation of it.


Applications & Priorities
-------------------------

The following sections list concrete problem domains that should be tackled, in order of priority:

### Higher Education Institution Identifiers

Given their crucial importance, we suggest that Higher Education Institution Identifiers be the first problem domain to be concretely addressed.
The following [whitepaper](Problem%20Domains/HEI%20Identifiers.md) discusses options for HEI Identifiers.

### Minimum Common Data Formats
An agreement would cover the minimum fields different data models should harmonise, for the purposes of promoting interoperability.  At European level, it might be useful to agree on minimum common data formats for describing:

1. Information on countries and their higher education system(s)
1. Basic information on higher education institutions
1. Information on study programmes
1. Information on quality assurance (of an institution or programme)
1. Information on student achievements (credits)
1. Information on a qualification awarded

### Course Identifiers

If HEI Identifiers are solved, it becomes easy to solve course identifiers, via a specification that sets a course identifier as HEI Identifier/Course Identifier. We therefore would propose addressing this issue after HEI Identifiers

Other problem domains should be added over time

<hr />

<span id="f1">\[1\]</span> see [BFUG Meeting 71 June 2020 - Draft 5 Rome Communiqué](http://www.ehea.info/Upload/BFUG_HR_UA_71_9_Draft_5_Rome_Communique.pdf)

<img src="https://www.eqar.eu/assets/uploads/2018/04/LogosBeneficairesErasmusLEFT_EN-e1524042594488.jpg" align="right" />
*The DEQAR CONNECT project is co-funded by the European Union's Erasmus+ programme. The EU support does not constitute an endorsement of the contents of this material, which reflects the views only of the authors, and the Commission cannot be held responsible for any use which may be made of the information contained herein.*

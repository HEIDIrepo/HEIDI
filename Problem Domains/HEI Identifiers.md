# HEI Identifiers Whitepaper

## Relevance

Higher education institutions (HEIs) are a pivotal enitity for many different systems and applications. Institutional identifiers are thus a matter of priority.

With less than 10000 HEIs in Europe the numbers are relatively managable, but yet large enough to warrant some standardisation to allow for data exchange without manual intervention or mapping.

## Existing systems

Various approaches already exist to identify higher education institutions in Europe:

| Identifier               | Maintained by         | Used in                | Link                                                                      | Comment                                              |
|:-------------------------|:----------------------|:-----------------------|:--------------------------------------------------------------------------|:-----------------------------------------------------|
| PIC                      | EU                    | EU programmes, European Student Card | [EU portal](https://ec.europa.eu/info/funding-tenders/opportunities/portal/screen/how-to-participate/participant-register) |     |
| Erasmus Institution Code | EU                    | Erasmus+               | [EU page](https://eacea.ec.europa.eu/erasmus-plus/actions/erasmus-charter_en)   |                                                |
| eIDAS identifier         | EU                    | EDCI                   | [EU page](https://ec.europa.eu/digital-single-market/en/trust-services-and-eid) | Just an organisational identifier. Not HE specific   |
| SCHAC                    | Géant                 | ELMO, Emrex, EWP       | [SCHAC](https://wiki.refeds.org/display/STAN/SCHAC)                       |                                                      |
| ETER ID                  | EU-funded consortium  | ETER, OrgReg, DEQAR    | [ETER](https://eter-project.com/#/home)                                   |                                                      |
| DEQARINST ID		   | EQAR		   | DEQAR		    | [DEQAR data set](https://www.eqar.eu/qa-results/get-data/download-data-sets/) | main need for HEIs not contained in ETER         |

The [EWP Registry Service](https://github.com/erasmus-without-paper/ewp-specs-api-registry/#registry-service) provides an accessible mapping between SCHAC, PIC and Erasmus codes for a number, but not all HEIs in Europe. The EU provides a [spreadsheet](https://eacea.ec.europa.eu/erasmus-plus/actions/erasmus-charter_en) of Erasmus Institution Codes, including the related PIC code.

Given that each organisation has their own approach how to deal with demographic changes (e.g. mergers), there is not necessarily a one-to-one relationship between different identifiers.

In conclusion, existing identifiers for HEIs in Europe are currently not fully articulated to each other.

## Use Cases

The following use cases should be made possible/be facilitated by an enhanced approach to HEI identifiers.

**NB: This is an initial collection of use cases. We aim to supplement those with contributions from stakeholders during the discussion. Use cases should be defined in line with [this template](../Supporting/UseCaseTemplate.md).**

### Cross-check Institution Data

**Actor:** HEI, recognition officer, student, employer

**Submitter:** [Colin Tück](https://github.com/ctueck)

**User Story:** The users receives data from or about a HEI, and wishes to automatically search another database for additional data about the HEI concerned.

For example, the user might recieve student mobility data, such as a transcript of records, via EMREX or EWP, or a qualification from a student applying for recognition. The user wants to acquire information on the sending institution's quality assurance status from DEQAR.

**Restrictions:** none

### Populate EDCI Accreditation Database

**Actor:** Europass National Offices

**Submitter:** [Anthony F. Camilleri](https://github.com/anthonycamilleri)

**User Story:** The user wishes to collect national data on courses, qualifications and institutional/programme accreditations, and upload these to Europass to power the 'course search', as well as the 'accreditation check' for digitially signed credentials. The identifiers used for data collection at national level should ensure no duplication of data, while the identifiers sent to Europass should resolve back to the institutions, and also not be duplicated with identififiers from other Member States/data suppliers.

**Restrictions:** All institutions in the database must be represented by a URI due to requirements arising from the [W3C Verifiable Credentials](https://www.w3.org/TR/vc-data-model/) standard.

### Correlate Datasets

**Actor:** researcher, policy maker, statistics office

**Submitter:** [Colin Tück](https://github.com/ctueck)

**User Story:** The user has data on a number of HEIs in Europe and wishes to correlate this with other data or statistics on the same HEIs, e.g. from ETER.

**Restrictions:** none

### List Higher Education Institutions

**Actor:** HEI, student, university staff

**Submitter:** [Jeroen van Lent](https://github.com/jeroenvl)

**User Story:** The user wishes to access a list of current Higher Education Institutions in Europe, and preferably also globally. This include names in English as well as in local language and also distinguish the business/brand name, should that be different from the legal name + official abbreviation. This list should be made available to a directory of HEIs as well as made available to various student information systems and student data exchange applications.

**Restrictions:** none

### Geographic Clustering

**Actor:** HEI, student, university staff

**Submitter:** [European University Foundation](https://github.com/EuropeanUniversityFoundation)

**User Story:** The user wishes to cluster HEIs by geographical location, preferably based on coordinates. (NUTS2 regions are not universally available beyond the EU.)

#### Automatic verification of accreditation

**Actor:** Supplier of digital credential services, EMREX

**Submitter:** [Geir Vangen](https://github.com/geirmv)

**User Story:** The user wishes to get an automatic check of the accreditation of a person’s digital credentials. This involves check of institution, study program, qualification, courses, modules etc. 

This is also a part of the user story regarding EDCI Accreditation Database. But this is a proposal for a standardized decentralized network of accreditation information, where data are governed locally (by e.g. Enic-Naric organizations) with the possibility of national or local storage of accreditation data. Both central and decentralized verification services should be able to use these local nodes to check accreditation, each node should operate independent of the rest of the network. These verification services should be open for use from any system or network handling digital credentials (Ex EMREX, EWP, Diploma registry services). When digitalizing diplomas, transcript of records etc, these data and surrounding services need to persist for many decades.

**Restrictions:** none (so far)

## Requirements

To be derived from use cases and discussed at first meeting.

## Options

To be elaborated and discussed after first meeting.


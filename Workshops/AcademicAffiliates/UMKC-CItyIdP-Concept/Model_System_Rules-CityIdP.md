Version 1.06c 
# Model System Rules

## Legal Notices

Intellectual Property: Massachusetts Institute of Technology, © 2013. Massachusetts Institute of Technology licenses distribution and re-use of this material under Creative Commons Attribution-ShareAlike 3.0 Unported License: http://creativecommons.org/licenses/by-sa/3.0/deed.en_US, provided the text of legal notices including attributions, disclaimers and document information are unchanged and conspicuously displayed on each copy or derivative works.

"MIT", "Massachusetts Institute of Technology", and its logos and seal are trademarks of the Massachusetts Institute of Technology. Except for purposes of attribution as required by our Creative Commons License, you may not use MIT’s names or logos, or any variations thereof, without prior written consent of MIT. You may not use the MIT name in any of its forms nor MIT seals or logos for promotional purposes, or in any way that deliberately or inadvertently claims, suggests, or in MIT's sole judgment gives the appearance or impression of a relationship with or endorsement by MIT.

Attributions and Disclaimer: This work is based upon work supported by the Defense Advance Research Project Agency (DARPA) and Space and Naval Warfare Systems Center Pacific under Contract N66001-11-C-4006. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the author(s) and do not necessarily reflect the views of the Defense Advance Research project Agency (DARPA) and Space and Naval Warfare Systems Center Pacific.

Document Information: Version 1.06; June 20, 2013; Comments to: daz@media.mit.edu; Authoritative stable release version of the System Rules is published at the MIT Human Dynamics Lab openPDS project site: http://openpds.media.mit.edu/#rules; The System Rules project background and news site: http://ecitizen.mit.edu/modelrules; The current exploratory drafts and alternative provisions under consideration in the MIT Human Dynamics Lab GitHub Repository: https://github.com/HumanDynamics/SystemRules

## Preface

This document provides Trust Framework System Rules for the provision of Personal Data and Individual Identity services. The architecture and model followed by these System Rules enables interoperability at the business, legal and technical dimensions, and ensures that each of those dimensions is expressly aligned, harmonized, and integrated.

Specifically, these System Rules anticipate and are tailored to support a prospective production grade roll out of openPDS and Funf software for Reality Analysis, and more generally, as an example of how System Rules following this model can enable and accelerate achieving the broader goal of a Personal Data Ecology. Please note that for purposes of presenting a complete and coherent reference example, “placeholders” and “hooks ” have been used for names of parties or business services. For future commercial or production grade use of these Rules, implementers would replace the example parties, service descriptions, etc., with the respective names and applicable terms specific to the business roles and relationships agreed among the parties.

# 1. BUSINESS RULES

## 1.1 Scope and Purpose

These System Rules apply to the use of the Personal Data and Individual Identity System by Individual Users, Third Party Service Providers and the System Provider, individually and in any combination. These Rules are intended and shall be interpreted to ensure that the access and interoperability enabled for access to and sharing of personal data is at all times subject to privacy protection and fair information practices. Further, these System Rules govern The Municipal OIDC Trust Framework and the use by all Parties and Roles  of OpenID 2.0 and OpenID Connect as described in Section 3, collectively called Municipal Identity (Muni-ID). This Trust Framework also applies to all non-Muni-ID users who connect to Muni-ID systems using the Muni-ID External Identity Federation.

[Commentary: The MITRE scope and the original PDS language are joined here. Possibly consider having both of those services expressed in the rules because of the consensus that the PDS is the final realization of both an integrated Trust Federation and the best way to provide notice and choice of data use.]

The primary purpose of the System is to enable a means for individual human beings to simply, efficiently, securely and effectively exercise their rights to store and keep private their own personal data and to share access to such data by their express consent and authorization through System Services. The System is specifically intended to empower individual users to not only grant or not grant such authorizations, but also to monitor, manage and modify or revoke such access over time. The simple, efficient, secure and effective Personal Data Services are also intended to enable Third Party Service Providers to provide added value to individual Participants and derive value from access to permission-based data access in an expanded marketplace. Leveraging the capability of API’s for Third Party apps under a common rule set and services enhances the value of the system to all parties while ensuring privacy.

The ancillary purpose of the System is to unify government and citizen interface into one portal. This will allow many government institutions to completely delegate citizen interaction to the System and thus relieve themselves of the burden of housing personally identifiable data, such as usernames and passwords. Further, the government institutions, jurisdictions, and political subdivisions can more efficiently, securely, and effectively implement and iterate digital services because the System provides universal standards and expectations. 

[Commentary: The above paragraph is an attempt to describe the purpose for the Municipalities or Government Entities that participate within the System. Obviously, there will need to more iterations later.]

The issuance of individual identity credentials and related System Services is likewise intended to empower individual Participant rights and expectations of autonomy and control of their own digital identity. The information comprising the digital identifiers, attributes, tokens and other similar identity data is also considered personal data of a particularly sensitive and valuable nature, hence a compatible and beneficial set of Services to be included within this System and subject to these Rules .

The focus of these Rules is to standardize essential interface and interoperability implementation requirements necessary to ensure expected outcomes by all Parties while encouraging wide latitude for individually agreed interactions and competitively evolving innovation. These System Rules are intended to provide a reliable and efficient method of achieving the purpose of the System.

## 1.2 Parties and Roles

These System Rules are applied by and to the Parties registered as current Participants in the System Registry. Each Party, in order to be approved as a Participant, must contractually assent to the Participation Agreement, including the Terms of Agreement corresponding to the Role or Roles that Party will conduct within the System and specifically including acceptance of the rights, obligations and functions allocated to the Role or Roles agreed by each Party:

### 1.2.1 Individual Participant

An individual human being who has contractually assented to Terms of Agreement and is a citizen holding a valid account with the Personal Data Store. An Individual Participant may use his or her account to request, accept and use a Grant of Authorization to access the Personal Data of another Principal Participant user.

Any individual human who contractually assents to the Terms of Agreement is eligible to apply for and hold an Account on the System. Services or other premium functions offered for free or other billing basis are available subject to fulfillment of applicable payment terms as agreed by the Individual User.

### 1.2.2 Principal Participant

An individual human who has contractually assented to Terms of Agreement and is a citizen holding a valid account with the Personal Data Store offered by the System Provider under these Rules. A Principal Participant may use his or her account to store his or her own Personal Data on the System and to Grant Authorization for accessing that Personal Data to Third Party Service Providers and/or to individual Participants.

### 1.2.3 System Provider

The Municipality, Government Subdivision, Jurisdiction, or Licensed Private Third Party responsible for the Personal Data System, comprised of the Personal Data Store and Services. The System Provider promulgates these System Rules.

### 1.2.4 Third Party Service Providers

The Party or Parties that operate and provide Third Party Services approved for use with the System and in accordance with these Rules. Only Third Party Providers that have been approved by the System Provider and contractually assented to the Participation Agreement, including the Terms of Agreement, are eligible to Participate in the System. Only an Approved Third Party Service Provider is eligible to receive the tokens necessary to use a Grant of Authorization by an Individual User or otherwise to use an Approved Scope and Grant Type for access of any kind to data or other resources within or through the System or otherwise subject to these Rules.

[Commentary: The below are possible parties for a Municipal IdP Use Case] 

### 1.2.5 Policy Authority 

The Municipality shall be the Policy Authority and is responsible for updating and interpreting this Trust Framework and designating or approving, directly or by delegated authority, the then current parties assuming the roles below. In commission of it’s duties as the Policy Authority the Municipality shall establish a Data Commission. There shall be 9 positions filled with the Mayor or a delegate of the Mayor’s, the City Manager or a delegate of the City Manager’s, the City Attorney or a delegate of the City Attorney’s, 2 City Council member’s or a delegate of their choosing, and 3 citizen’s appointed by the Mayor. The scope of the of the Data Commission is to review policy and determine whether or not the system is fulfilling stated policy objectives. Further, the Data Commission must set forth and monitor a mechanism by which the public at large, or individuals, may hold the Muni-ID Trust Framework accountable. 

### 1.2.6 System Operator 

The Municipality shall be the system operator and is responsible for implementing and administering the Muni-ID.

### 1.2.7 Identity Provider

The Municipality shall be the Identity Provider is responsible for issuing a Primary Credential or a Derived Federated Identity Credentials for Users. 

A White Listed Identity Provider system is a service provider that has been approved by the System Operator as a pre-authorized Identity Provider such that Muni-ID Relying Party sites may provide automatic authorization on first and all subsequent access to Users of Derived Federated Credentials issued by that Identity Provider.

### 1.2.8 User Authority

Any Jurisdiction that currently issues credentials to Users and is approved by the System Operator may be a User Authority and is responsible for authorizing the issuance of Primary Credentials to Users.

### 1.2.9 User

A User is a single human who authenticates to any system covered by this Trust Framework, either using a Primary or Derived Federated Credential.

### 1.2.10 Relying Party

A Relying Party is a service provider that accepts or has accepted a Derived Federated Credential issued by an Identity Provider for the purpose of authenticating a User.

A White Listed Relying Party system is a service provider that has been approved by the System Operator as a pre-authorized Relying Party such that Muni-ID users are provided automatic authorization on first and all subsequent access to one or more Relying Party sites.

### 1.2.11 Certification Assessor

The Data Commission shall select a Certification Assessor who is an independent party and is responsible for certifying or recommending certification of Identity Providers, User Authorities and/or Relying Parties according to criteria set or adopted by the System Operator.

[Commentary: The above provisions are from the MITRE example provided by Dazza Greenwood. The following is from the Commentary section of that model; “MITRE is pursuing Federal Identity, Credential, and Access Management (FICAM) accepted certification at this time for its OpenID 2.0 service for the purpose of gaining more information about this process and evaluating how best to adopt or adapt this process for use in its internal determination of which external parties to federate with and specifically which parties to add to White Lists.” That might be something a Municipality might wish to also pursue.]

[Commentary: Until now all sources of agreements have determined certification of parties, either white, grey, black, or rainbow, based on the characteristics of the party. We believe that is half of the analysis. First the characteristic of the party must be ascertained then the characteristic of the imminent transaction must be determined. A party might be white listed as a matter of policy, but that status might change depending on the data sought.]

### 1.2.12 White, Black and Grey Lists

#### 1.2.12.1 Grey List

Grey Listed sites include any Identity Provider or Relying Party that implements the standards in Section * and that has not been added to a White List or Black List by the System Operator. Any Grey Listed Relying Party may accept a Derived Federated Credential from any User and any User may use a Derived Federated Credential to access the site of any Grey Listed Relying Party.

If an Identity Provider is Grey Listed, then the Relying Party makes the decision on a per use or other basis whether to accept and rely upon credentials issued by that Identity Provider. If a Relying Party is on a Grey List then the User makes the decision whether to authorize the use of their Derived Federated Credential to access the Relying Party site.

#### 1.2.12.2 White List

The System Operator, by approval of or delegated authority by the Policy Authority, may add a Relying Party site to the Muni-ID White List, thereby allowing automated authorization for MITRE Users.

#### 1.2.12.3 Black List

The System Operator may determine whether a site is in violation of these rules or otherwise disapproved for federation, and upon such determination may add that site to the Muni-ID Black List, thereby preventing a Muni-ID User from using their Derived Federated Credential to access such site and preventing Derived Federated Credentials from Black Listed Identity Providers from being used to access Muni-ID Relying Party sites under this Trust Framework.

### 1.2.13 Certification

Certification is a material consideration favoring the System Operator decision on inclusion of parties to a White List, but is neither required nor sufficient. 

[Commentary: This will be subject to further policy considerations.]


## 1.3 System Services

### 1.3.1 Service Lifecycle

Approval by the System Provider is required as a precondition to the offering of any Service though this System. Any approved Service that is currently offered through the System is enumerated in Rule 1.3.2 and is available in accordance with the technical specifications defined under Rule 3.2 and subject to all relevant Rules and used subject to the relevant provisions of the Terms of Agreement of any Participant using the Service.

### 1.3.2 System Service

The following Services are approved and provisioned for use by or with the System, subject to these Rules:

#### 1.3.2.1 "Personal Data Storage and Archive" services,

#### 1.3.2.2 “Personal Data Collection and Import” services,

#### 1.3.2.3 "Personal Data Sharing Control" services,

#### 1.3.2.4 “ Analytics and Visualization" services, 

#### 1.3.2.5 “Personal Data Export” Services, and

#### 1.3.2.6  “Personal Data Deletion” services.

## 1.4 Recording and Reporting

Any Recording or Reporting requirement under these Rules must result in the logging of the required record at the System Registry (or other facility provided by the System Provider) within the time prescribed or if no time is prescribed or if extenuating circumstances are permitted under these Rules, it shall be logged as soon as practicable.

Every Third Party Service must be implemented so as to ensure creation, accuracy, integrity, preservation and accessibility of Required Records such that upon review an objectively verifiable account can be made of the relevant transactions or other actions, the salient terms (i.e. the data accessed, modified or deleted or other essential terms) the parties involved, the relevant times, and the applicable Terms of Agreement and Terms of Authorization.

## 1.5 Use of System Logo and Marketing

Any use of the System Logo, and any marketing, advertising or other public communications referencing approved Third Party Provider status or other affiliation with this System is prohibited unless explicitly permitted in the applicable Terms of Agreement and only for such time as the Terms of Agreement are in effect.

# 2. LEGAL RULES

## 2.1 Scope and Application

### 2.1.1 Promulgation of Rules

The content comprising the “System Rules” duly promulgated by the System Provider in accordance with these Rules, is the formal and binding normative version of these Rules as of the moment of publication and until the moment of publication of a subsequent version or for such period of time as provided under these Rules.

Neither this Trust Framework, nor any course between the Parties hereunder, shall constitute or create a partnership, joint venture, principal-agent relationship or employer-employee relationship between the Parties.

### 2.1.2 Authoritative Rules and Incorporation by Reference

The authoritative current version of the Trust Framework System Rules can be found at www.municipality.gov [note actual URL to be determined]. These Rules, including all documents explicitly Incorporated by Reference, provide standard default terms for use of the External Identity Federation, but in the event of a conflict between the terms of an existing contract between parties governing the terms of access to relevant applications or services, then the terms of the existing contract shall govern.

When the text of these Rules explicitly refers to a “document Incorporated by Reference” and includes a URL to the authoritative version of that document, then the content of that document shall have the same force and effect as if directly published within these Rules.

### 2.1.3 Order of Precedence

In the event of a conflict between the provisions of these Rules and the provisions of the Terms of Agreement between any Parties to these Rules, then the provisions of these Rules shall prevail.

In the event of a conflict between the terms of these Rules and an Independent Commercial Contract between any Parties to these Rules, then, as between a Principal Participant and a Third Party Service Provider, the provisions of the applicable Terms of Authorization incorporated by reference into the Parties Terms of Agreement shall prevail, and otherwise the provision of the Independent Commercial Contract shall prevail.

In the event of a conflict between the terms of these Rules and the applicable Jurisdiction’s Law, then the Jurisdiction’s Law shall prevail.

## 2.2 Rights and Obligations of Participants

### 2.2.1 General Obligation

All Participants agree to abide by the terms and act in accordance with these Rules and adhere to respect each Principal Participant’s ownership and control rights to their own Personal Data stored in or accessible through this System.

### 2.2.2 Protection and Promotion of Individual Participant Identity and Data Rights

The System Provider is responsible for safeguarding the Individual Participant’s elemental rights to his or her own individual identity and ownership of their personal data and may as appropriate protect and defend such rights and as needed represent the interests of such Participant vis-a-vis external parties when such rights are threatened.

### 2.2.3 Minimum Required Obligations of Third Party Providers to individual Participants

Each Third Party Provider agrees to comply with the Terms of Authorization between itself and each individual Participant from whom the Third Party Provider has received a Grant of Authorization for access to personal data of such Participant

To ensure the purpose of this System and expectations of individual Participants are met, every Third Party Provider must correctly and completely implement the Approved Scopes and Grant Types and corresponding obligations and stipulations for each such Scope and Grant. Furthermore, every Third Party Provider must agree to accept that the legal rights and obligations corresponding to each Approved Scopes and Grant Types are contractually enforceable by the Participant that has granted such Authorization to such Third Party Provider or by the System Provider as a Third Party Beneficiary. Failure to comply with these requirements renders any Third Party Provider ineligible for Participation and subject to termination, suspension, or a review process at the sole discretion of the System Provider.

To be eligible for approval by the System Provider, a prospective Third Party Provider must submit a Third Party Provider Application, including truthful, accurate and complete information. Every Third Party Provider must contractually assent to abide by and in practice adhere to these Rules. Manual Registration of a Third Party Service, Client or Other App is required. Any approved Third Party Provider may accept individual Participant Grants of Authorization corresponding to one or more Approved Scope and Grant Type for access to that Participant’s Personal Data.

Any approved Third Party Provider may establish such additional terms of service, including with respect to billing, liability and service quality, with individual Participants of the System, as the parties may agree provided that no contractual term or other obligation shall be enforceable against any individual Participant to the extent the obligation arises from or applies to that Participant ‘s Grant of Authorization to the Third Party Provider and is inconsistent with any provision of these Rules.

## 2.3 Logging and Reporting

### 2.3.2 Recording With System Registry

The Required Record of any transaction or other action subject to a Reporting requirements under Rule 1.4 or otherwise required under these Rules must be logged with the System Registry (or other facility provided by the System Provider) and a copy preserved by the Party responsible. The following actions are subject to a logging requirement: • Promulgation and Amendment to these Rules • Activation, Status Change or Closure of Participant Account • Each Grant of Authorization by a Principal Participant, including Modification or Revocation of Such Grant of Authorization • Supported Scopes of User Authorization, Including Modification or Removal of such Scopes • System Interfaces for REST calls, including Modification or Removal of any Such Specification • Provision, Modification or Removal of a System Service or Component

## 2.4 Liability and Indemnification

Under these Rules, no Individual User shall be liable to nor shall owe any obligation of indemnity to any other party for any actions that were conducted in compliance with these Rules. The applicable provisions of the Terms of Agreement regarding liability, indemnity, damages and warranties shall apply to Parties to such agreements, subject to the Order of Precedence defined in Rule 2.1.3.

THE MUNICIPALITY OR OTHER PARTIES MAKES NO WARRANTY, EXPRESS OR IMPLIED, AS TO THE ACCURACY, CAPABILITY, EFFICIENCY, MERCHANTABILITY, OR FUNCTIONALITY OF MUNI-ID OR MUNI-ID EXTERNAL IDENTITY FEDERATION OR ANY INFORMATION OR SERVICES COMPRISING OR RELATED TO MUNI-ID OR MUNI-ID EXTERNAL IDENTITY FEDERATION. IN NO EVENT WILL THE MUNICIPALITY OR PARTIES BE LIABLE FOR ANY GENERAL, CONSEQUENTIAL, INDIRECT, INCIDENTAL, EXEMPLARY, OR SPECIAL DAMAGES, EVEN IF MUNI-ID HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.

ANY NON-MUNI-ID PARTY SUBJECT TO THIS TRUST FRAMEWORK AGREES TO INDEMNIFY AND HOLD HARMLESS MUNI-ID, ITS AFFILIATES AND SUBSIDIARIES, AND THEIR RESPECTIVE DIRECTORS OR TRUSTEES, OFFICERS, EMPLOYEES AND AGENTS FROM ANY AND ALL INJURIES, LOSSES, CLAIMS AND DAMAGES TO ANY PERSON OR PROPERTY UNDER ANY THEORY OF LIABILITY AND IRRESPECTIVE OF THE CAUSE OF SAID LIABILITY, AND ALL COSTS AND EXPENSES INCLUDING WITHOUT LIMITATION, ATTORNEYS' FEES AND ANY OTHER LIABILITIES INCURRED BY MUNI-ID AS A RESULT OF ANY NEGLIGENT OR WILLFUL ACTION OR OMISSION OF SUCH PARTY, HIS/HER EMPLOYEES OR AGENTS, OR ARISING OUT OF OR RESULTING IN ANY MANNER IN WHOLE OR IN PART FROM THE SUCH PARTY’S USE OF OR RELIANCE UPON MUNI-ID OR MUNI-ID EXTERNAL IDENTITY FEDERATION OR ANY INFORMATION OR SERVICES COMPRISING OR RELATED TO MUNI-ID OR MUNI-ID EXTERNAL IDENTITY FEDERATION.

## 2.5 Intellectual Property

### 2.5.1 Trademark and License in System Trustmark and Logo

Use of the System trademarks or logos must comply with the Trustmark and Branding Policy and License Agreement. No Party may use or display any trademark or logo without explicit permission and license to do so. Parties that are engaged in a process of applying for participation are not parties to the License Agreement and not permitted to use such trademarks or logos. Parties that were Participants at one time but whose Participation status is suspended or terminated, whether voluntarily or involuntarily, are likewise not permitted to use or display the System trademarks or logos, and must cease any use that had previously been permitted in accordance with the license terms.

### 2.5.2 Copyright and License in System Rules

These Rules are available to be downloaded, stored, transmitted and duplicated on a royalty free, perpetual and global basis, under a Creative Commons Attribution-Share Alike 3.0 Unported License. The System Provider shall ensure the Creative Commons license is applied to these Rules.

## 2.6 Amendment

These Rules may be amended from time to time by the System Provider in accordance with the Notice requirements of Section 

## 2.7 Notice

Amendment of a Rule or change to the System that is not material is effective when duly promulgated by the System Provider. An affected Participant is entitled to receive 30 calendar days advance notice of any amendment of a Rule or change to the System that constitutes material change, unless an emergency condition requires a shorter period or no notice.

## 2.8 Other Legal Terms

The Terms of Agreement, including the Terms of Authorization, as executed or adopted by each Participant include more specific terms and may include varying provisions, subject to Rule 2.1.3 governing Order of Precedence. The terms defining and governing the overall business relationship and legal rights, expectations or other responsibilities and duties of the Participants are addressed in one or more Independent Commercial Contracts executed or adopted by Participants, subject to Rule 2.1.3.

## 2.9 Order of Precedence

In the event Muni-Id and another Party subject to this Trust Framework and any documents or policies incorporated by reference also are subject to another contract or other enforceable agreement and there is an inconsistency or conflict between terms of any of those documents, the inconsistency or conflict shall be resolved in accordance with the following order of precedence:

- The Contract or other enforceable agreement between Muni-ID and the other Party or Parties
- Any Muni-ID policy of other official document incorporated by reference into this Trust Framework
- The Terms of Use and/or Muni-ID Privacy Policy of the site being accessed with a Derived Federated Credential
- This Trust Framework
- Any other documents, including technical standards, protocols or industry guidelines

# 3. TECHNICAL RULES

## 3.1 Scope and Application

### 3.1.2 Technical Use Cases

The following use cases are supported under this Trust Framework: [TBD]

[Commentary: For so long as Muni-ID is an early-stage policy initiative, it is premature to focus on detailed documentation of supported use cases. However, this draft Trust Framework anticipates a future state at which external and internal parties will seek to implement and interoperate with Muni-ID External Identity Federation services and the important role of this document to facilitate and regulate adoption. To that end, the types of technical use cases that would be relevant and constructive to detail in the future are noted below.

 - Muni-ID User Logs Into Grey Listed Relying Party
 - Muni-ID User Logs Into White Listed Relying Party
 - Muni-ID User Logs Into Black Listed Relying Party
 - Non-Muni-ID User Logs Into Muni-ID External Identity Federation Enabled Site
 - Non-Muni-ID CAC User Logs Into Muni-ID External Identity Federation Enabled Site
 - Muni-ID Relying Party Site Implements Muni-ID External Identity Federation Access
 - Non-Muni ID Identity Provider Added to Muni-ID External Identity Federation White List
 - Non-Muni-ID Relying Party Site Accepts Muni-ID User Login]

### 3.1.3 Technical Architecture

[Commentary: In this section, if desired, Muni-ID can describe its technical architecture. The current diagrams depicting initial architectural approach are included in Addendum ** below.]

### 3.1.4 Supported Standards

The System supports and depends upon the following Standards and relies upon conformance with and interoperability based upon correct implementation of these standards:

#### 3.1.4.1 OAuth2

The System Authorization and Resource servers support the final version of the AUth2 Core as defined at http://tools.ietf.org/html/draft-ietf-oauth-v2

The System Authorization and Resource servers support the final version of the AUth2 Bearer Token usage as defined at Bearer: http://tools.ietf.org/html/draft-ietf-oauth-v2-bearer

#### 3.1.4.2 Authoritative Normative Sources

OAuth2: Core: http://tools.ietf.org/html/draft-ietf-oauth-v2 Bearer: http://tools.ietf.org/html/draft-ietf-oauth-v2-bearer

JSON Object Signing and Encryption: JWT (tokens): http://tools.ietf.org/html/draft-ietf-oauth-json-web-token JWS (signing): http://tools.ietf.org/html/draft-ietf-jose-json-web-signature JWE (encryption): http://tools.ietf.org/html/draft-ietf-jose-json-web-encryption JWK (keys): http://tools.ietf.org/html/draft-ietf-jose-json-web-key JWA (algorithms): http://tools.ietf.org/html/draft-ietf-jose-json-web-algorithms

#### 3.1.4.3 OpenID 2.0

##### 3.1.4.3.1 Protocol Version

###### 3.1.4.3.1.1 All Identity Providers and Relying Parties MUST support the OpenID 2.0 Authentication protocol as defined in http://openid.net/specs/openid-authentication-2_0.html

##### 3.1.4.3.2 Attributes

###### 3.1.4.3.2.1 All Identity Providers MUST support the OpenID 2.0 Attribute Exchange 1.0 protocol as defined in http://openid.net/specs/openid-attribute-exchange-1_0.html

###### 3.1.4.3.2.2 Identity Providers MUST make attributes available using the following schema URLs from exampleschema.org

Base URL: http://exampleschema.org/
Preferred username: http://exampleschema.org/namePerson/friendly
First name: http://exampleschema.org/namePerson/first
Last name: http://exampleschema.org/namePerson/last
Full display name: http://exampleschema.org/namePerson
Business email address: http://exampleschema.org/contact/email
Business phone: http://exampleschema.org/contact/phone/business

#### 3.1.4.4 OpenID Connect

##### 3.1.4.4.1 Protocol Version

###### 3.1.4.4.1.1 OpenID Connect Final Standard

All Identity Providers and Relying Parties MUST support the OpenID Connect final standard as defined by http://openid.net/connect

##### 3.1.4.4.2 The Muni-ID OpenID Connect server supports the final version of the OpenID Connect protocol as defined by http://openid.net/connect Protocol Profile.

The Muni-ID OpenID Connect server will support the following flows and options

 - Basic client profile (code flow) as defined by http://openid.net/specs/openid-connect-basic-1_0.html including:

	* Authorization Code flow
	* UserInfo Endpoint with "openid" schema
	* Asymmetrically signed id_token (with RSA)
	* Additionally, the Muni-IP server supports the following optional components of OpenID Connect:

 - Asymmetrically signed Request Objects (via RSA)

	* Server keys published via JWK and X509
	* Access tokens signed with RSA by server
	* Dynamic client registration
	* Server discovery

##### 3.1.4.4.3 Claims

The following claims are supported from the UserInfo Endpoint with semantics defined in http://openid.net/specs/openid-connect-messages-1_0.html

 - user_id, guaranteed unique and stable per user
 - name
 - given_name
 - family_name
 - preferred_username
 - email
 - email_verified
 - phone_number

These are simply a starting point for claims. A major reason for using Municipalities as the Identity Provider and System Operator is that the list of standard claims is only limited by the what the institutions and the citizen-users agree is appropriate.

[Commentary: For the use case of the Employee Liquor Permit Application Use case thee following are sample claims that ONLY a Muni-ID and its trust federation populate with other government entities could provide; 

Resident of Kansas City
 1) Locale, See attached OICD Standard Physical Address
 2) Birthdate
	a. Data: Birthdate
        b. Type: String
        c. Description:End-User's birthday, represented as an ISO 8601:2004 [ISO8601‑2004] YYYY-MM-DD format. The year MAY be 0000, indicating that it is omitted. To represent only the year, YYYY format is allowed. Note that depending on the underlying platform's date related function, providing just year can result in varying month and day, so the implementers need to take this factor into account to correctly process the dates.
 3) Employment Eligibility
        a. Data: Employment Eligibility
        b. Type: String
        c. Description: Document and identifying numbers from the document proving eligibility to work in the US. Could be the following documents Social Security Card without employment restriction, U.S. Passport or Passport Card, Permanent Resident Card (i.e., Green Card), Foreign Passport with I-551 stamp MRIV, Employment Authorization Card, Form I-20 accompanied by Form I-94 or Form I-94A, Form DS-2019 accompanied by Form I-94 or Form I-94A, or Form I-94 or Form I-94A Arrival/Departure Record.
        d. Data: Employment Eligibility Verification
        e. Type: Boolean
        f. Description: True if the End-User's employment eligibility has been verified; otherwise false. When this Claim Value is true, this means that the OP took affirmative steps to ensure that the End-User had documentation at the time the verification was performed. The means by which a employment eligibility is verified is context-specific, and dependent upon the trust framework or contractual agreements within which the parties are operating. 
 4) Aged 18- 20 years
        a. Data: Birthdate Verification
        b. Type: Boolean
        c. Description: True if End-User has aged 18 years, but less than 20 years, otherwise false. This means the OP has taken affirmative steps to verify against another URI that the End-User has aged between 18-20 years. 
 5) Aged 21 years
        a. Data: Birthdate Verification
        b. Type: Boolean
        c. Description: True if the End-User has aged 21+ years, otherwise False. This means the OP has taken affirmative steps to verify against another URI that the End-User has aged 21 years.
 6) Dangerous Offender (need more guidance from the City on what that means)
        a. Should replicate Felony Claims below
 7) Categorical Bar Felony (there are several felonies that trigger a categorical bar from ever receiving the permit, there would need to be a separate claim for each one: murder, voluntary manslaughter, forcible rape, forcible sodomy, kidnapping, false imprisonment, first degree child molestation, second degree child molestation, sexual abuse or an attempt to commit any of the preceding crimes)
        a. Data: Felony
        b. Type: Boolean
        c. Description:  False if End-User’s felon status has been verified as non-felon, True if there End-User’s felon status is verified as felon; otherwise False. When this claim is True it means that the End-User provided necessary data to establish felon status and the OP took affirmative measures to confirm the data. 
 8) Conditional Bar for Crimes Against a Person Felony (This felony is bar only for a certain period of time and only for felonies that are classified as crimes against a person, which would need further clarification)
        a. Data: Felony Crime Against a Person
        b. Type: Boolean
        c. Description:  False if End-User’s felon status has been verified as a non felony crime against a person, True if there End-User’s felon status is verified as felony crime against a person; otherwise False. When this claim is True it means that the End-User provided necessary data to establish felony crime against a person status and the OP took affirmative measures to confirm the data.
        d. Data: Felony Crime Against a Person Conviction Date
        e. Type: String
        f. Description: End-User's conviction date, represented as an ISO 8601:2004 [ISO8601‑2004] YYYY-MM-DD format. The year MAY be 0000, indicating that it is omitted. To represent only the year, YYYY format is allowed. Note that depending on the underlying platform's date related function, providing just year can result in varying month and day, so the implementers need to take this factor into account to correctly process the dates.
        g. Data: Felony Crime Against a Person Conviction Date Verification
        h. Type: Boolean
        i. Description: False if End-User’s felony crime against a person conviction date has been verified as longer than 8 years, True if there End-User’s felony crime against a person conviction date is within 8 years of the date of application; otherwise False. When this claim is True it means that the End-User provided necessary data to establish felony crime against a person status and the OP took affirmative measures to confirm that the user was convicted of a felony crime against a person offense listed above, less than 8 years for the date of application.
        j. Data: Felony Crime Against a Person Release Date
        k. Type: String
        l. Description: End-User's release date, represented as an ISO 8601:2004 [ISO8601‑2004] YYYY-MM-DD format. The year MAY be 0000, indicating that it is omitted. To represent only the year, YYYY format is allowed. Note that depending on the underlying platform's date related function, providing just year can result in varying month and day, so the implementers need to take this factor into account to correctly process the dates.
        m. Felony Crime Against a Person Release Date Verification
        n. Type: Boolean
        o. Description: False if End-User’s felony crime against a person release date has been verified as longer than 8 years ago, True if there End-User’s felony crime against a person release date is within 8 years of the date of application; otherwise False. When this claim is True it means that the End-User provided necessary data to establish felony crime against a person status and the OP took affirmative measures to confirm that the user was released from prison for one of the above felony crime against a person conviction, less than 8 years ago from the date of application.
9) Conditional Bar for Drug Related Felonies (Here is the list provided in the application; involving the sale or possession of controlled substances or illegal drugs or narcotics, or intent to distribute controlled substances or illegal drugs or narcotics)
        a. Data: Drug Related Felony
        b. Type: Boolean
        c. Description:  False if End-User’s felon status has been verified as non drug related felony, True if the End-User’s drug related felony status is verified; otherwise False. When this claim is True it means that the End-User provided necessary data to establish drug-related felony status and the OP took affirmative measures to confirm the data.
        d. Data: Drug Related Felony Conviction Date
        e. Type: String
        f. Description: End-User's conviction date, represented as an ISO 8601:2004 [ISO8601‑2004] YYYY-MM-DD format. The year MAY be 0000, indicating that it is omitted. To represent only the year, YYYY format is allowed. Note that depending on the underlying platform's date related function, providing just year can result in varying month and day, so the implementers need to take this factor into account to correctly process the dates.
        g. Data: Drug Related Felony Conviction Date Verification
        h. Type: Boolean
        i. Description: False if End-User’s Drug related drug related felony conviction date has been verified as longer than 4 years from the date of the application, True if there End-User’s drug related felony conviction date is within 4 years of the date of application; otherwise False. When this claim is True it means that the End-User provided necessary data to establish drug related felony status and the OP took affirmative measures to confirm that the user was convicted of a felony offense listed above, less than 4 years from the date of the application.
        j. Data: Felony Crime Against a Person Release Date
        k. Type: String
        l. Description: End-User's release date, represented as an ISO 8601:2004 [ISO8601‑2004] YYYY-MM-DD format. The year MAY be 0000, indicating that it is omitted. To represent only the year, YYYY format is allowed. Note that depending on the underlying platform's date related function, providing just year can result in varying month and day, so the implementers need to take this factor into account to correctly process the dates.
        m. Felony Crime Against a Person Release Date Verification
        n. Type: Boolean
        o. Description: False if End-User’s drug related felony release date has been verified as longer than 4 years from the date of the application, True if there End-User’s drug related felony release date is within 4 years of the date of application; otherwise False. When this claim is True it means that the End-User provided necessary data to establish drug related felony status and the OP took affirmative measures to confirm that the user was released from prison for one of the above drug related felony convictions, less than 4 years from the date of the application.
10) Permit 
        a. Data: Permit Number
        b. Type: String
        c. Description: The associated number within regulated industries. 
        d. Data: Permit Status
        e. Type: String
        f. Description: 
        g. Data: Permit Status
        h. Type: Boolean
        i. Description: True if status of the permit is current, false if the status of the permit is revoked. The means by which a permit status is verified is context-specific, and dependent upon the trust framework or contractual agreements within which the parties are operating.

### 3.1.5 White, Black and Grey Lists

The technical configuration accompanying implementation of White and Black list determinations made in accordance with this Trust Framework System Rules are noted in this section.

#### 3.1.5.1 Grey List

No additional configuration is required for any Grey List site or service.

#### 3.1.5.2 White Listed Identity Providers

White Listed Identity Providers have their Trust Root for OpenID 2.0 or Issuer for OpenID Connect reflected in the Relying Party.

#### 3.1.5.3 White Listed Relying Parties

White Listed Relying Parties have their Trust Root for OpenID 2.0 and/or their Client ID for OpenID Connect configured in the Relying Party system.

[Commentary: When a Relying Party has provided a “Login With MITRE Button”, in effect that Relying Party has White Listed Muni-ID as an Identity Provider.]

#### 3.1.5.4 Black Listed Identity Providers

Black Listed Identity Providers have their Trust Root for OpenID 2.0 or Issuer for OpenID Connect configured to be denied in Relying Party system.

#### 3.1.5.5 Black Listed Relying Parties

Black Listed Relying Party’s have their Trust Root for OpenID 2.0 and their redirect URI for OpenID Connect configured to be denied in the Relying Party system.

## 3.2 Service Provision and System Components

Services offered through the System are enumerated in Rule 1.3.

### 3.2.1 Personal Data services

A Principal Individual User may import Personal Data and other records to their Personal Data Store that is hosted at the OpenPDS operated by System Provider by use of a Third Party Provider that has an approved service for that transaction.

### 3.2.2 System Components

In addition to Services and Interfaces, the System includes the following modular components.

#### 3.2.2.1 openPDS

The authoritative version and build of openPDS software supported and implemented in the System under these Rules is located at https://github.com/humandynamics.

#### 3.2.2.2 Funf Mobile Sensor Framework

The Mobile Health Funf Mobile Sensor Framework is open source software available for inclusion in Android apps available for use by Principal Individual Users. The specifications of the current supported version and build of this software and links to documentation is available at http://funf.org.

## 3.3 Approved Scopes of User Authorization and Grant Types

Only requests for access to Personal Data that conform with the defined Approved Scopes and Grant Types are permitted or supported under these Rules.

## 3.4 Security and Resilience

Passwords: Only an Individual User’s Account password can decrypt that user’s Personal Data or other sensitive information, and System Provider does not store this password. As a result, no one—not even System Provider employees—can see the sensitive information a Principal User places in the System. If a Principal User forgets his or her password and needs to reset it, the System Provider shall delete that user’s sensitive information for his or her own protection. System Provider must also have mechanisms in place to stop brute force attacks on passwords, and offer multi-factor authentication and secure password recovery

Servers: Personal Data is stored in a major U.S. server storage facility that has 24/7 security guards and biometric security for entry, has been issued an SSAE16 Type II SOC 1 Report, is a PCI Security Standards Council Member, is Safe Harbor Certified, and offers protection via firewalls, its own intrusion detection systems, and other measures.

Data Storage: All personal data are encrypted in database servers, including by the use of 256-bit AES encryption and RSA 2048 asymmetric key encryption. Personal Data containing sensitive information must be encrypted uniquely, in order to add an extra layer of security. Non-sensitive information may only be accessed through a Principal User-chosen password that must not be stored by the System Provider. While technically possible for a small and limited group of System operations employees to access non-sensitive information, they are strictly forbidden from doing so, consistent with System Provider policies and these Rules, unless required by law, and access to System Provider servers is carefully logged.

Secure Coding and Data Management Practices: System Provider shall not use insecure third-party delivery networks, and must ensure that Principal User Personal Data is never exposed. System Provider is not permitted to see Principal User Personal Data even in the context of crash reports. In addition, System Provider must not use data de-duplication methods, which can raise security and privacy concerns.

Security Testing and Certificates: System Provider conducts audits of System security, including penetration testing by outside firms. System Provider uses SSL certificates from VeriSign and GeoTrust. In addition, System Provider constantly monitors the System for potential threats and vulnerabilities.

Principal’s Control Their Personal Data: Only a Participant account holder can grant individuals, companies or applications access to his or her Personal Data and permanently delete or export his or her Personal Data. Third Party Providers are not allowed to track Participants while they are on the System, and the System Provider does not track Participants when they leave the System or a mobile app that is part of the System.

System Provider Employees: All System Provider employees undergo background checks going back 10 years as a condition of employment, and all technical employees receive security training.

## 3.5. Information Security

### 3.5.1. Token Signing

All OpenID Connect and OAuth2 tokens MUST be signed with the public key of the Identity Provider that has issued the token.

### 3.5.2. JWK Discoverability

All public keys MUST be discoverable as per the JWT Web Key (JWK) specification.

## 3.6. Meta-Data Exchange

### 3.6.1 All OpenID 2.0 servers MUST be discoverable from the public internet using the Yadis protocol defined in OpenID 2.0

### 3.6.2 All OpenID Connect servers MUST be discoverable from the public internet using the Simple Web Discovery (SWD) and XRD/Webfinger protocols as defined in OpenID Connect.

### 3.6.3 All OpenID Connect servers MUST allow for manual registration of OpenID Connect clients.

### 3.6.4. All OpenID Connect servers SHOULD allow for dynamic client registration.

[Commentary: The purpose of using “SHOULD” in this rule is because in the specification the criteria is a “MAY” and this feature is not always implemented. However, we do favor its use.]

### 3.7. Event Logging

### 3.7.1. Identity Provider Event Logging

An Identity Provider MUST log the following events:

 - User approves a site
 - User logs in to an Identity Provider
 - User uses an Identity Provider to log into a Relying Party
 - User denies log in to a Relying Party
 - User revokes access to a Relying Party

### 3.7.2. The System Operator shall maintain records of the Identity Provider log files related to MITRE Users and required under Section 3.6.1 in accordance with MITRE Records Management Procedure IM 4.3.1.1.

### 3.7.3. White Listed Relying Party Event Logging

A White Listed Relying Party MUST log the following events:

 - User selects an Identity Provider to login to a Relying Party
 - User uses an Identity Provider to login to a Relying Party
 - User denies the authentication transaction

## 3.8 Testing and Change Management

The System makes available a sandbox and test harness to Third Party Provider applicants to test the readiness for business, legal and technical interoperability with other Participants and for Participants to text readiness of modified or new Services, Transactions or other functions.

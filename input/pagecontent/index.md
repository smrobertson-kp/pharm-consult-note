### Purpose

The scope of this implementation guide is to provide IG to the pharmacy sector of the healthcare industry on the use of the [HL7 Implementation Guide for CDA® Release 2: Consolidated CDA Templates for Clinical Notes (US Realm) Standard for Trial Use Release 2.1](http://www.hl7.org/implement/standards/product_brief.cfm?product_id=408) (C-CDA Template) and [C-CDA on FHIR 1.1.0 - (FHIR R4) STU Release 1.1 Consultation Note Profile](http://www.hl7.org/fhir/us/ccda/StructureDefinition-Consultation-Note.html) (FHIR Profile) in creating a Pharmacist Consultation Note. The Pharmacist Consultation Note is used for exchange of the pharmacist’s recommendations with the appropriate long term post acute care (LTPAC) facility staff and the physician(s) of record for the patient. This paper is based on the C-CDA Template and FHIR Profile.

This IG is intended to be used in conjunction with the specifications as defined in the C-CDA Template and FHIR Profile. The NCPDP Long Term and Post Acute Care (LTPAC) Work Group (WG14) Consultant Pharmacist Interoperability Task Group has reviewed the C-CDA templates and FHIR Profile; and found the content and functionality of the C-CDA Template and FHIR Profile meet the requirements of the structured documentation of the Consultant Pharmacist’s Consultation Note. The C-CDA Template and FHIR Profile provide information regarding levels of constraint, conformance statements, conformance verbs, cardinality, vocabulary conformance, and null flavor that are pertinent to this IG.

Matters such as the maintenance and storage of medication and storage equipment (e.g., refrigeration, humidity and temperature control, etc.), medication security and access protocols, etc., are not within the scope of this IG document.

### Audience

The audience for this recommendation for use of this IG document is the architects, developers and implementers of HIT systems in the US Realm to meet health IT certification requirements for exchange of patient clinical data particularly among pharmacists, LTPAC facilities as well as other healthcare providers, and caregivers. All participants in the healthcare team will benefit from the implementation of these recommendations.

### Overview

Consultant pharmacists play a pivotal role in the long term and post-acute care arena in helping patients/residents attain and maintain the highest practicable level of functional status and preventing or minimizing medication-related adverse consequences. For the purpose of this IG document, the term patient will be used when referring to residents of LTPAC facilities. The consultant pharmacist’s primary focus is the nursing home population, which may be quite diverse, including geriatric patients as well as individuals of any age with special needs, such as those who are immunocompromised, have end stage renal disease, spinal cord or closed head injuries, neurological syndromes, etc. These patients tend to have multiple risk factors including medication-related adverse consequences. Although the intent of this IG document is for consultant pharmacist in the LTC setting, this can also be applied to other care settings (e.g., medical at home, assisted living, home health care).

Medications are used for their therapeutic benefits in diagnosing, managing, and treating acute and/or chronic conditions, as well as for maintaining and/or improving a patient’s functional status. Information about indications for use, potential medication irregularities or adverse consequences (such as symptoms of tardive dyskinesia, dizziness, anorexia, or falls) may be attainable only by talking to the staff, reviewing the medical record, and observing and speaking with the patient. However, electronic health and medication records and other available technology may permit the pharmacist to conduct some components of the review from outside the facility.

The following information in this overview references the [Centers for Medicare and Medicaid Services (CMS) State Operations Manual Appendix PP - Guidance to Surveyors for Long Term Care Facilities Transmittals for Appendix PP, Revision 173, November 22, 2017](https://www.cms.gov/Regulations-and-Guidance/Guidance/Manuals/downloads/SOM107ap_pp_Guidelines_ltcf.pdf). The [cms.gov](https://www.cms.gov) website should be consulted for any updates to regulatory requirements.

The pharmacist must review each patient’s medication regimen at least monthly in order to identify irregularities as well as clinically significant risks and/or adverse consequences resulting from or associated with medications. The requirement for the medication regimen review (MRR) applies to each patient, including patients who:

1. Are receiving respite care;
2. Are at the end of life or have elected the hospice benefit and are receiving respite care;
3. Have an anticipated stay of less than 30 days; or
4. Have experienced a change in condition.

#### Notification of Irregularities Identified in the MRR

The timeliness of notification of irregularities depends on factors including the potential for or presence of serious adverse consequences; for example, immediate notification is indicated in cases of bleeding in a patient who is receiving anticoagulants or of possible allergic reactions to antibiotic therapy. If no irregularities were identified during the review, the pharmacist includes a signed and dated statement to that effect. The facility and the pharmacist may collaborate to identify the most effective means for assuring appropriate notification. This notification may be done electronically.

The pharmacist does not need to document a continuing irregularity in the report each month if the pharmacist has deemed the irregularity to be clinically insignificant or evidence of a valid clinical reason for rejecting the pharmacist’s recommendation was provided. In this situation, the pharmacist need only reconsider annually whether to report the irregularity again or make a new recommendation.

The intent of this requirement is that each patient’s entire medication regimen be managed and monitored. Monitoring is the ongoing collection and analysis of information (such as observations and diagnostic test results) and comparison to baseline data.

The regulations associated with medication management include consideration of:

- Indications for use of medication (including initiation or continued use of antipsychotic medication);
- Monitoring for efficacy and adverse consequences;
- Dose (including duplicate therapy);
- Duration;
- Tapering of a medication dose/gradual dose reduction for antipsychotic medications; and,
- Prevention, identification, and response to adverse consequences.

#### Response to Irregularities Identified in the MRR

Throughout this IG, a response from a physician regarding a medication problem implies appropriate communication, review, and patient management, but does not imply the physician must necessarily order tests or treatments recommended or requested by the staff, unless the physician determines those are medically valid and indicated. For those issues that require physician intervention, the physician either accepts and acts upon the report and potential recommendations or rejects all or some of the report and provides a brief explanation of why the recommendation is rejected, such as in a dated progress note. It is not acceptable for a physician to document only that he/she disagrees with the report, without providing some basis for disagreement.

If there is potential for serious harm and the attending physician does not concur with or take action on the report, the facility and the pharmacist should contact the facility’s medical director for IG and possible intervention to resolve the issue. In cases where the attending physician is also the medical director, the facility should have alternate procedures in place to resolve the situation. For those recommendations that do not require physician intervention, such as monitoring vital signs or weights, the director of nursing or designated licensed nurse addresses and documents action(s) taken.

The recommendations provided for use of the C-CDA templates and FHIR Profile to construct the Pharmacist Consultation Note are designed to:

- support the consultant patient specific recommendations for LTPAC facilities
- to meet the regulatory requirements for nursing facilities
- support LTPAC needs
- support care coordination

In addition to the stated C-CDA templates and FHIR Profile components, the HL7 process allows for inclusion of other section level and entry level templates, as needed, to fully meet the documentation needs of the consultant pharmacist’s recommendations.

The consultant pharmacist recommendations as reported in the Consultation Note (using either or both C-CDA or FHIR) potentially provide medication-related input into the patient’s care plan goals, health concerns and interventions. The Pharmacist Consultation Note is integral to the development and maintenance of the LTPAC resident’s longitudinal care plan.

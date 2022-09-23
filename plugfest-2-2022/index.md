# JFF & VC-EDU 
## Interoperability Plugfest 2

### August-November 2022

**Demo Event: November 14, 2022 (9 am Pacific Time) - Computer History Museum, Mountain View, CA, USA**

The purpose of this event is to issue W3C Verifiable Credentials in the Open Badges v3 format and Decentralized Identifiers to wallets using protocols that are popular in the education and workforce ecosystem.

**Kick-Off Meeting September 14, 2022**
* [Slides](https://docs.google.com/presentation/d/1oAV3hFt7R-HSlKSvJojigxYOwnjLkDF5XW1NJJGiDqA/edit#slide=id.g35f391192_00)
* [Zoom Recording](https://us06web.zoom.us/rec/share/PMW689VGovd3svrp7qgju1Vc0dM2y4k2ye4cdvdlAXSFE6cQ8WnWUEOEiBu35ZyO.cwymES5swaLA92Qi) passcode: 6U+e#p%M

---

* [Requirements](#requirements)
* [Participation Overview](#participation-overview)
* [Frequentky Asked Questions](#frequently-asked-questions)
* [Resources](#resources)

---

## Requirements

### Wallet Requirements

* Display: Verifiable credential (OBv3) from at least two different credential issuers
* Display: badge image, issuer name, achievement name, achievement description, achievement criteria
* Optional Display: issuer logo & other Open Badges v3 terms

### Issuer Requirements

* Issue: Verifiable credential (OBv3) to at least two different wallets (using [Verifiable Credentials HTTP API v0.3 - VC-API](https://w3c-ccg.github.io/vc-api/), [OpenID for Verifiable Credential Issuance](https://openid.net/specs/openid-4-verifiable-credential-issuance-1_0.html, [WACI-DIDComm Interop Profile](https://identity.foundation/waci-didcomm/))
* Optional Display: badge image, issuer name, issuer logo, achievement name, achievement description, achievement criteria, & other Open Badges v3 terms

---

## Participation Overview
### Registering for Plugfest #2

Please complete this form by Friday, September 9, 2022, 12 PM ET
[https://forms.gle/Y1b38UwLHVLFwP898](https://forms.gle/Y1b38UwLHVLFwP898)

We will notify participants of their successful participation no later than Monday, September 12, 2022, 11 AM ET.

If you need assistance with registration, please contact Joan Lee, [jlee@jfflabs.org](maito:jlee@jfflabs.org).

### Plugfest #2 Activities

| Date                | Activity |
|---------------------|----------|
| August 8, 2022      | Open Call for PlugFest 2 Participation / AMA at weekly VC-EDU meeting
| September 9, 2022   | Last day to register to participate **Complete registration form by 12 PM ET**
| September 12, 2022  | All participants notified by 11 AM ET
| September 14, 2022  | PlugFest 2 Kick-off Meeting, 11 AM ET
| September 28, 2022  | PlugFest 2 Technical Meeting, Time TBD
| October 12, 2022    | PlugFest 2 Technical Meeting, Time TBD
| October 26, 2022    | PlugFest 2 Technical Meeting, Time TBD
| November 9, 2022    |[tentative] Demo videos due
| November 14, 2022   | PlugFest 2 Demo Day: IIW and virtual [details tbd]

## Frequently Asked Questions

### Questions About Eligibility

**If I am a wallet implementer and did not participate in PlugFest 1, am I eligible to participate in PlugFest 2?**

Yes!  We are excited that you are joining us in this important work.  While it is not necessary for you to have participated in PlugFest 1, we are requiring that all participants in PlugFest 2 successfully demonstrate that their wallet can hold a verifiable credential in the OBv3 format.  This is the credential format that we will use for PlugFest 2.

The PlugFest team will issue a JFF credential to your wallet using the DID method of your choice.  Please provide the information request in the registration form.  If you are unclear how to proceed, please send an email to Joan Lee, [jlee@jfflabs.org](maito:jlee@jfflabs.org).

**If I am a credential issuing platform and did not participate in PlugFest 1, am I eligible to participate in Plugfest 2?**

Yes!  We are excited that you are joining us in this important work.  Credential issuing platforms were not eligible to participate in PlugFest 1, so there are no new additional requirements for their participation in PlugFest 2.

**What is an example of a credential issuing platform?**

Credential issuing platforms issue verifiable credentials as a service to any wallet, including those not provided by their own platform.

**Are educational institutions eligible to participate in PlugFest 2 as a credential issuing platform?**

Educational institutions, training providers, and other credential providers are eligible to participate if the credential issuing service is universally available to others outside their organization.  

### Questions About Technical Requirements

**What are the technical requirements for wallet implementers?**

* Display: Verifiable credential (OBv3) from at least two different credential issuers
* Display: badge image, issuer name, achievement name, achievement description, achievement criteria
* Optional Display: issuer logo & other Open Badges v3 terms


**What are the technical requirements for credential issuing platforms?**

* Issue: Verifiable credential (OBv3) to at least two different wallets (using [Verifiable Credentials HTTP API v0.3 - VC-API](https://w3c-ccg.github.io/vc-api/), [OpenID for Verifiable Credential Issuance](https://openid.net/specs/openid-4-verifiable-credential-issuance-1_0.html, [WACI-DIDComm Interop Profile](https://identity.foundation/waci-didcomm/))
* Optional Display: badge image, issuer name, issuer logo, achievement name, achievement description, achievement criteria, & other Open Badges v3 terms

**Can we participate if we have not yet decided which protocol to implement?**

Yes!  The VC-EDU plugfest team is excited to learn more about the different wallet/issuing solutions and are happy to provide technical support and resources to teams who are in the process of selecting a protocol.  Please indicate your interest using the form or by using the VC-EDU mailing list [https://lists.w3.org/Archives/Public/public-vc-edu/](https://lists.w3.org/Archives/Public/public-vc-edu/). 

**Can we participate if we do not intend to implement one of the three protocols (VC-API/CHAPI, OpenID Connect, DID-Comm Presentation Exchange)?**

In order to participate, you must select at least one of the three protocols.

**Can we use a different verifiable credential that is not an open badge (OBv3)?**

For the purpose of this plugfest, we will be focusing on a single achievement verifiable credential that all wallets are able accept (OBv3).  Participants in PlugFest 2 are welcome to make suggestions on other verifiable credential formats in coordination.  If there is demand for these formats by wallet implementers within the PlugFest 2 cohort, the plugfest team is open to considering these other credentials.

**Are we required to use an Open Badge provided by the plugfest organizers like we did in Plugfest 1 ?**

No, we will provide an example that you may use but you may also use your own baadges as long as they are compliant with [Open Badges 3.0](https://imsglobal.github.io/openbadges-specification/ob_v3p0.html)

**Will credential issuers be required to use DIDs?**
Yes.

**Will DID Authentication be required?**
Yes. Note that DID authentication does not reuqire using DIDAuth protocol. It's expected that DID authentication will be dictated by protocol choice.

**Who decides which DID method to use - wallet or credential issuing platforms?**

This will be a collaborative decision between wallets & issuers.

### Questions About Funding

**Will there be funding to support technical development or team coordination activities for this Plugfest?**

$10,000 will be available to each organization (wallet/issuer/both) that demonstrates successful execution of the technical requirements.  As in PlugFest 1, participants will be required to submit a video on ahead of demo day (November 14, 2022).  Additional information will be provided in September.

---

## Resources

* [DID Actor](https://api.did.actor/)
* [DIDComm](https://didcomm.org/)
* [DID DIF Universal Resolver](https://dev.uniresolver.io/)
* [Hosted platform to resolve and manage DIDs](https://godiddy.com/)
* [VC-API](https://github.com/w3c-ccg/vc-api/)
* [CHAPI - Credential Handler API](https://chapi.io)
* [OIDC- OpenID for VCs](https://openid.net/wordpress-content/uploads/2022/05/OIDF-Whitepaper_OpenID-for-Verifiable-Credentials_FINAL_2022-05-12.pdf)
* [Open Badges 3.0](https://imsglobal.github.io/openbadges-specification/ob_v3p0.html)
* [Plugfest 1](https://w3c-ccg.github.io/vc-ed/plugfest-1-2022/)
* [Plugfest 1 Participants](https://w3c-ccg.github.io/vc-ed/plugfest-1-2022/participants.html)
* Protocols:
  * [Verifiable Credentials HTTP API v0.3 - VC-API](https://w3c-ccg.github.io/vc-api/)
  * CHAPI Quick Reference: [for Issuers](https://chapi.io/developers/issuers), [for Digital Wallets](https://chapi.io/developers/wallets), [for Verifiers](https://chapi.io/developers/verifiers)
  * [OpenID for Verifiable Credential Issuance](https://openid.net/specs/openid-4-verifiable-credential-issuance-1_0.html)
  * [WACI-DIDComm Interop Profile](https://identity.foundation/waci-didcomm/)
* [Universal Wallet](https://w3c-ccg.github.io/universal-wallet-interop-spec/)
* [VC Implementation Guide](https://www.w3.org/TR/vc-imp-guide/)
* [VC Issuing Protocols Overview - slides](https://docs.google.com/presentation/d/12K8EIzFjzsC2i1WwfzggsXISGXZ64f1xwHJ5qO5rylc/edit#slide=id.p)

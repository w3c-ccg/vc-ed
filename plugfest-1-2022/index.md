# JFF & VC-EDU 
## Interoperability Plugfest #1 

### May/June 2022

### Resources

* [Kick-off Meeting Deck](https://docs.google.com/presentation/d/1YoS3est-YnWO1tI7JjJDjSPSnIXJNon_TFosKyneaJg/edit?usp=sharing)
* [VC Implementation Guide](https://www.w3.org/TR/vc-imp-guide/)
* [Plugfest Open Badges v3 context](https://w3c-ccg.github.io/vc-ed/plugfest-1-2022/jff-vc-edu-plugfest-1-context.json)
* [Open Badges 3.0](https://imsglobal.github.io/openbadges-specification/ob_v3p0.html)
* [Universal Wallet](https://w3c-ccg.github.io/universal-wallet-interop-spec/)
* [DCC Learner Credential Wallet](https://github.com/digitalcredentials/learner-credential-wallet)
* [DCC Repository](https://github.com/digitalcredentials)
* [DCC Open Badges 3.0 Context NPM Module](https://github.com/digitalcredentials/open-badges-context)
* [DID Actor](https://api.did.actor/)
* [Hosted platform to resolve and manage DIDs](https://godiddy.com/)
* [DID DIF Universal Resolver](https://dev.uniresolver.io/)

### Requirements of Plugfest 1

* Display: VC (Open Badge 3.0)
* Display includes: VC required fileds plus badge image, issuer name, achievement name, achievement description, achievement criteria
* Optional: issuer logo & other Open Badges v3 terms
* Stretch: badge verification

### Examples

#### Simple Open Badge as a VC
<pre>
{
  "@context": [
    "https://www.w3.org/2018/credentials/v1",
    "https://w3c-ccg.github.io/vc-ed/plugfest-1-2022/jff-vc-edu-plugfest-1-context.json"
  ],
  "type": [
    "VerifiableCredential",
    "OpenBadgeCredential"
  ],
  "issuer": {
    "type": "Profile",
    "id": "did:key:z6MkrHKzgsahxBLyNAbLQyB1pcWNYC9GmywiWPgkrvntAZcj",
    "name": "Jobs for the Future (JFF)"
  },
  "issuanceDate": "2022-05-01T00:00:00Z",
  "credentialSubject": {
    "type": "AchievementSubject",
    "id": "did:key:123",
    "achievement": {
      "type": "Achievement",
      "name": "Our Wallet Passed JFF Plugfest #1 2022",
      "description": "This wallet can display this Open Badge 3.0",
      "criteria": {
        "type": "Criteria",
        "narrative": "The first cohort of the JFF Plugfest 1 in May/June of 2021 collaborated to push interoperability of VCs in education forward."
      }
    }
  },
  "proof": {
    "type": "Ed25519Signature2018",
    "created": "2022-05-26T20:31:11Z",
    "verificationMethod": "did:key:z6MkrHKzgsahxBLyNAbLQyB1pcWNYC9GmywiWPgkrvntAZcj#z6MkrHKzgsahxBLyNAbLQyB1pcWNYC9GmywiWPgkrvntAZcj",
    "proofPurpose": "assertionMethod",
    "jws": "eyJhbGciOiJFZERTQSIsImI2NCI6ZmFsc2UsImNyaXQiOlsiYjY0Il19..e7vekXR-WCFJGoPo9ClxVv_zaauy9NtbP6N-frqPh9aoDpG2UwvkljvTMAelvfep54blrEfxFMFrIdq2jqaVDA"
  }
}
</pre>
File: [plugfest-1-ex-1.json](plugfest-1-ex-1.json)

#### Bonus Badge with Images
<pre>
{
  "@context": [
    "https://www.w3.org/2018/credentials/v1",
    "https://w3c-ccg.github.io/vc-ed/plugfest-1-2022/jff-vc-edu-plugfest-1-context.json"
  ],
  "type": [
    "VerifiableCredential",
    "OpenBadgeCredential"
  ],
  "issuer": {
    "type": "Profile",
    "id": "did:key:z6MkrHKzgsahxBLyNAbLQyB1pcWNYC9GmywiWPgkrvntAZcj",
    "name": "Jobs for the Future (JFF)",
    "url": "https://www.jff.org/",
    "image": "https://kayaelle.github.io/vc-ed/plugfest-1-2022/images/JFF_LogoLockup.png"
  },
  "issuanceDate": "2022-05-01T00:00:00Z",
  "credentialSubject": {
    "type": "AchievementSubject",
    "id": "did:key:123",
    "achievement": {
      "type": "Achievement",
      "name": "Our Wallet Passed JFF Plugfest #1 2022",
      "description": "This wallet can display this Open Badge 3.0",
      "criteria": {
        "type": "Criteria",
        "narrative": "The first cohort of the JFF Plugfest 1 in May/June of 2021 collaborated to push interoperability of VCs in education forward."
      },
      "image": "https://w3c-ccg.github.io/vc-ed/plugfest-1-2022/images/plugfest-1-badge-image.png"
    }
  },
  "proof": {
    "type": "Ed25519Signature2018",
    "created": "2022-05-26T20:43:50Z",
    "verificationMethod": "did:key:z6MkrHKzgsahxBLyNAbLQyB1pcWNYC9GmywiWPgkrvntAZcj#z6MkrHKzgsahxBLyNAbLQyB1pcWNYC9GmywiWPgkrvntAZcj",
    "proofPurpose": "assertionMethod",
    "jws": "eyJhbGciOiJFZERTQSIsImI2NCI6ZmFsc2UsImNyaXQiOlsiYjY0Il19..i6qtkTNW1lWzsPhqUVyU_80x-wifVuvdMqII5TIYpjWsp0fJ19r7gJReOpTvSMenWxd7rXj9RiyiT1xwB9OVBA"
  }
}
</pre>
File: [plugfest-1-ex-2.json](plugfest-1-ex-2.json)

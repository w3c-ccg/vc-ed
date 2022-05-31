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

#### Open Badge 3.0 with Badge Image & Required Fields
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
      },
      "image": "https://w3c-ccg.github.io/vc-ed/plugfest-1-2022/images/plugfest-1-badge-image.png"
    }
  },
  "proof": {
    "type": "Ed25519Signature2018",
    "created": "2022-05-27T15:08:03Z",
    "verificationMethod": "did:key:z6MkrHKzgsahxBLyNAbLQyB1pcWNYC9GmywiWPgkrvntAZcj#z6MkrHKzgsahxBLyNAbLQyB1pcWNYC9GmywiWPgkrvntAZcj",
    "proofPurpose": "assertionMethod",
    "jws": "eyJhbGciOiJFZERTQSIsImI2NCI6ZmFsc2UsImNyaXQiOlsiYjY0Il19..-1WePLNRNxXq2wOJeLOsxf7kXQqQfQovWYqF6TZATp0CWnn1LL5ABWmsY_EcwtWXfh5KywsuTW_b0re2Y3epDQ"
  }
}
</pre>
File: [plugfest-1-ex-1.json](plugfest-1-ex-1.json)

#### Open Badge 3.0 with Optional & Required Fields
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
    "created": "2022-05-31T21:09:29Z",
    "verificationMethod": "did:key:z6MkrHKzgsahxBLyNAbLQyB1pcWNYC9GmywiWPgkrvntAZcj#z6MkrHKzgsahxBLyNAbLQyB1pcWNYC9GmywiWPgkrvntAZcj",
    "proofPurpose": "assertionMethod",
    "jws": "eyJhbGciOiJFZERTQSIsImI2NCI6ZmFsc2UsImNyaXQiOlsiYjY0Il19..Q05Nb7ufRWi8b8MO11einZZzRgwU9iauqiKoB-tKCGRUIGWTM_-HUQMXsSE9rYm3wuv45qa5gl4TIl5lwWgvDA"
  }
}
</pre>
File: [plugfest-1-ex-2.json](plugfest-1-ex-2.json)

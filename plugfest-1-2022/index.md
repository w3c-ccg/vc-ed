# JFF & VC-EDU 
## Interoperability Plugfest #1 

### May/June 2022

### Resources

* [VC Implementation Guide](https://www.w3.org/TR/vc-imp-guide/)
* [Plugfest Open Badges v3 context](https://w3c-ccg.github.io/vc-ed/plugfest-1-2022/jff-vc-edu-plugfest-1-context.json)
* [Open Badges 3.0](https://imsglobal.github.io/openbadges-specification/ob_v3p0.html)
* [Universal Wallet](https://w3c-ccg.github.io/universal-wallet-interop-spec/)
* [DCC Learner Credential Wallet](https://github.com/digitalcredentials/learner-credential-wallet)
* [DCC Repository](https://github.com/digitalcredentials)
* [DID Actor](https://api.did.actor/)
* [Hosted platform to resolve and manage DIDs](https://godiddy.com/)
* [DID DIF Universal Resolver](https://dev.uniresolver.io/)

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
      "id": "did:key:z6Mkv8wY2XpNF48tFHomipRnh6eBNT1H7YB53yLNK2NSJKmH",
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
    "created": "2022-05-20T14:01:27Z",
    "verificationMethod": "did:key:z6MktiSzqF9kqwdU8VkdBKx56EYzXfpgnNPUAGznpicNiWfn#z6MktiSzqF9kqwdU8VkdBKx56EYzXfpgnNPUAGznpicNiWfn",
    "proofPurpose": "assertionMethod",
    "jws": "eyJhbGciOiJFZERTQSIsImI2NCI6ZmFsc2UsImNyaXQiOlsiYjY0Il19..tGwSg54AHnN4EIZrvDVSXbPh952dHFTnxmwlXuNsS3yi-IxWp1AMth0BgkSZBIlBTRsFb0T4GRaIf2ZIJuvqDg"
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
      "id": "did:key:z6Mkv8wY2XpNF48tFHomipRnh6eBNT1H7YB53yLNK2NSJKmH",
      "name": "Jobs for the Future (JFF)",
      "url": "https://www.jff.org/",
      "image": "https://w3c-ccg.github.io/vc-ed/plugfest-1-2022/images/JFF_LogoLockup.png"
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
    "created": "2022-05-19T20:48:35Z",
    "verificationMethod": "did:key:z6MktiSzqF9kqwdU8VkdBKx56EYzXfpgnNPUAGznpicNiWfn#z6MktiSzqF9kqwdU8VkdBKx56EYzXfpgnNPUAGznpicNiWfn",
    "proofPurpose": "assertionMethod",
    "jws": "eyJhbGciOiJFZERTQSIsImI2NCI6ZmFsc2UsImNyaXQiOlsiYjY0Il19..eTt6kQDHbIOUrZNnQwqFWS00eSEyZRBRuG1abs4sAPkSqa5BUz0X_gWO7vw2aDFwWfO6_2EyOfVD36i96XuKAg"
  }
}
</pre>
File: [https://kayaelle.github.io/vc-ed/plugfest-1-2022/plugfest-1-ex-2.json](https://kayaelle.github.io/vc-ed/plugfest-1-2022/plugfest-1-ex-2.json)

# Plugfest 1 

## May/June 2022

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
    "https://kayaelle.github.io/vc-ed/plugfest-1-2022/jff-vc-edu-plugfest-1-context.json"
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
      "image": "https://kayaelle.github.io/vc-ed/plugfest-1-2022/images/plugfest-1-badge-image.png"
    }
  },
  "proof": {
    "type": "Ed25519Signature2018",
    "created": "2022-05-19T20:30:01Z",
    "verificationMethod": "did:key:z6MktiSzqF9kqwdU8VkdBKx56EYzXfpgnNPUAGznpicNiWfn#z6MktiSzqF9kqwdU8VkdBKx56EYzXfpgnNPUAGznpicNiWfn",
    "proofPurpose": "assertionMethod",
    "jws": "eyJhbGciOiJFZERTQSIsImI2NCI6ZmFsc2UsImNyaXQiOlsiYjY0Il19..kCvMNnX8Hm1nEdf4HNWVxDUJ3TCfoyZopiUclTy-ASlBLW_i-mZQNSn8jh2eYAfhzG6mKJqYFikQyvao3MYzCg"
  }
}
</pre>
File: [https://kayaelle.github.io/vc-ed/plugfest-1-2022/plugfest-1-ex-2.json](https://kayaelle.github.io/vc-ed/plugfest-1-2022/plugfest-1-ex-2.json)

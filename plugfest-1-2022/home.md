# Plugfest 1 

## May/June 2022

#### Examples

##### Simple Open Badge as a VC
`
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
      "id": "did:key:z6Mkv8wY2XpNF48tFHomipRnh6eBNT1H7YB53yLNK2NSJKmH"
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
    "created": "2022-05-19T19:37:47Z",
    "verificationMethod": "did:key:z6MktiSzqF9kqwdU8VkdBKx56EYzXfpgnNPUAGznpicNiWfn#z6MktiSzqF9kqwdU8VkdBKx56EYzXfpgnNPUAGznpicNiWfn",
    "proofPurpose": "assertionMethod",
    "jws": "eyJhbGciOiJFZERTQSIsImI2NCI6ZmFsc2UsImNyaXQiOlsiYjY0Il19..dEt4UQIzoQkS3yO89KnNSQBxCecNr98JUjZTjos5eQUNcRfW6xNbwMTjGciICXtBYdD6Mn7DJeBd4yf_i_QzAQ"
  }
}`
File: 

##### Bonus Badge with Images
`
`
File: 

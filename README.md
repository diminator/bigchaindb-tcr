# BigchainDB Token-Curated Registry
Simple TCR on BigchainDB

## Motivation
Framework to create TCRs on BDB

Each TCR contains:
- a label / schellingpoint
- proposals
- challenges
- votes

## Data Structure

### Label
```json
{
  "namespace": "<URI>",
  "min_deposit": "<int>",
  "min_vote": "<int>"
}
```

### Proposal
```json
{
  "namespace": "<URI>",
  "registry_id": "<ID>",
  "deposit": "<int>",
  "description": "<string>"
}
```

### Challenge
```json
{
  "namespace": "<URI>",
  "proposal_id": "<ID>",
  "deposit": "<int>"
}
```

### Vote
```json
{
  "namespace": "<URI>",
  "challenge_id": "<ID>",
  "deposit": "<int>",
  "deposit": "<boolean>"
}
```

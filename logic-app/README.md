# Azure Billing Records Archival Solution

![Architecture Diagram](./docs/architecture-diagram.png)

## Key Features
- Daily archival of records older than 3 months
- Hierarchical storage in Blob Storage (`/year/month/record_id.json`)
- Automatic deletion from Cosmos DB post-archival
- Failure logging and retry mechanism

## Implementation Steps

### 1. Pre-requisites
- Azure Service Principal with Contributor permissions
- Existing Cosmos DB and Blob Storage accounts

### 2. Deploy Logic App

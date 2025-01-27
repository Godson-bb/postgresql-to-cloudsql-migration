# PostgreSQL to Google Cloud SQL Migration
[![Cloud Migration](https://img.shields.io/badge/Google_Cloud-Database_Migration-%234285F4?logo=google-cloud)](https://cloud.google.com/database-migration)

## 📌 Overview
Migration of `masteryhive-staging-db` (PostgreSQL 13.16) to Google Cloud SQL using Database Migration Service (DMS).

**Key Features**:
- Zero-downtime cutover
- Automated validation scripts
- Cost-optimized Cloud SQL configuration

## 🚀 Quick Start
### Prerequisites
- Google Cloud Account with billing enabled
- PostgreSQL 13.16+ source database
- `gcloud` CLI installed

### Migration Steps
1. Clone this repo:
   ```bash
   git clone https://github.com/godsonbb/postgres-to-cloudsql-migration.git

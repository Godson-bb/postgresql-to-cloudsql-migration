# 🚀 PostgreSQL to Google Cloud SQL Migration: Zero Downtime with Google DMS  
*A comprehensive guide to migrating PostgreSQL databases to Google Cloud SQL using Database Migration Service (DMS)*  

![Google Cloud SQL + PostgreSQL](https://img.shields.io/badge/Google_Cloud-PostgreSQL-%234285F4?logo=google-cloud&logoColor=white)  
*Tools used: Google Data migration Services, Cloud SQL, PostgreSQL 13.16, IAM, Cloud Monitoring*

---

## 📋 Project Overview  
**Role**: Data Engineer @ MasteryHive  
**Objective**: Migrate `masteryhive-staging-db` (PostgreSQL 13.16) to **Google Cloud SQL** with:  
- ✅ Zero downtime  
- ✅ Full data integrity  
- ✅ Cost optimization via managed services  

---

## 🛠️ Step-by-Step Migration Process  

### 1. Pre-Migration Preparation  
#### 🔍 Compatibility Checks  
- Verified PostgreSQL 13.16 ↔ Cloud SQL compatibility (supported versions 10-15).  
- Audited tables (e.g., `UserProject`, `ActionLog`) for unsupported extensions.  

#### ⚙️ PostgreSQL Configuration  
```ini
# postgresql.conf
wal_level = logical
max_replication_slots = 10
max_wal_senders = 10

###GCP Setup

    Project: masteryhive-cloud-migration

    APIs Enabled: DMS, Cloud SQL, Compute Engine, Cloud Storage

    IAM Roles: datamigration.admin, cloudsql.editor, storage.admin

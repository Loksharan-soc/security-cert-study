# Backups

## Overview

Backups are copies of data stored separately to protect against data loss from hardware failure, accidental deletion, cyberattacks, or disasters. They are a critical component of data protection and recovery strategies.

---

## Backup Types

| Type                | Description                                              | Use Case                                      |
|---------------------|----------------------------------------------------------|-----------------------------------------------|
| **Full Backup**     | Complete copy of all data.                               | Baseline backups, long-term storage.          |
| **Incremental Backup** | Copies only data changed since the last backup (full or incremental). | Saves time and storage, requires all increments to restore. |
| **Differential Backup** | Copies data changed since last full backup.            | Faster restore than incremental, larger backups. |
| **Snapshot**         | Point-in-time image of data or system state.             | Quick recovery, often used in virtual environments. |

---

## Backup Storage Options

- **Onsite**: Fast recovery but vulnerable to local disasters.
- **Offsite**: Protects against site-wide failures.
- **Cloud Backup**: Scalable, accessible, but dependent on internet and third-party security.
- **Hybrid**: Combines onsite and offsite for balance.

---

## Backup Strategies

| Strategy              | Description                                            |
|-----------------------|--------------------------------------------------------|
| **3-2-1 Rule**        | 3 copies of data, on 2 different media, 1 offsite copy. |
| **Regular Scheduling** | Daily, weekly, or monthly backups based on data criticality. |
| **Encryption**        | Protect backups against unauthorized access.          |
| **Verification**      | Test backups regularly to ensure data integrity.       |

---

## Considerations

- Backup window (time allowed for backup operations).
- Retention policies (how long backups are kept).
- Compliance requirements for data protection.

---

## Summary

A robust backup strategy ensures data availability and recoverability, minimizing the impact of data loss events and supporting business continuity.

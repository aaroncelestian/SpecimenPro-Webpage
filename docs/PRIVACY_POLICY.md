# Privacy Policy for SpecimenPro

**Last Updated: November 6, 2025**

## Introduction

SpecimenPro ("we," "our," or "the app") is committed to protecting your privacy. This Privacy Policy explains how SpecimenPro collects, uses, stores, and protects your information when you use our mobile application.

## App Versions

SpecimenPro is available in two versions:

- **SpecimenPro Lite** (Free): Access to all features with limits on collection creation and objects per collection
- **SpecimenPro Full** (One-time purchase): Unlimited collections and objects

Both versions have identical privacy practices. Upgrading to Full version does not change how your data is collected, stored, or used.

## Information We Collect

### Data You Provide

SpecimenPro collects and stores the following information that you directly provide:

- **Collection Information**: Collection names, dates, collector names, and collection types
- **Specimen Data**: Object numbers, specimen IDs, metadata, tags, and custom field data
- **Photos**: Images you capture or select, including drawer photos, object photos, detail photos, and custom photo types
- **Voice Notes**: Audio recordings you create and their associated titles
- **Location Data**: GPS coordinates and location information you manually enter for field collections
- **QR Codes**: QR code data you generate or scan for specimen identification
- **Event Participation**: When you participate in virtual events (mineral shows, fossil fairs), your progress and collected specimens are stored locally

### Automatically Collected Data

- **Device Information**: The app may access your device's camera and microphone (with your permission) to capture photos and voice notes
- **File System Access**: The app accesses your device's local storage to save and retrieve database files

### Purchase Information

When you purchase the Full version upgrade:

- **Payment Processing**: All payment transactions are processed by Apple through the App Store. We do not collect, store, or have access to your payment information (credit card numbers, billing addresses, etc.)
- **Purchase Verification**: The app verifies your purchase status through Apple's StoreKit framework to determine your app version (Lite or Full)
- **Purchase Records**: Apple maintains records of your purchases. We only store a local flag on your device indicating whether you have purchased the Full version
- **Install Date**: For grandfathering purposes, the app records the first launch date locally on your device to determine if you are eligible for automatic Full version access

## How We Use Your Information

SpecimenPro uses your information solely for the following purposes:

1. **Data Management**: To store, organize, and manage your specimen collections
2. **Export/Import**: To enable you to backup, export, and import your data
3. **QR Code Generation**: To create QR codes for specimen identification and tracking
4. **Local Storage**: All data is stored locally on your device in a SQLite database
6. **Events**: To fetch and display virtual event information (mineral shows, fossil fairs) and track your participation progress
7. **Purchase Verification**: To verify your Full version purchase status through Apple's StoreKit and enforce appropriate feature limits
8. **Grandfathering**: To determine if you installed the app before the Lite version was introduced and automatically grant Full version access

## Data Storage and Security

### Local Storage

- **All specimen data is stored locally on your device** in an SQLite database
- Data is saved in your device's app-specific documents directory
- Your specimen data is never transmitted to external servers
- Event information is downloaded from our server but your event progress is stored locally only
- Your data remains on your device unless you explicitly export or share it

### Data Security

- The app uses iOS security features to protect your data
- Database files are stored in the app's sandboxed environment
- Access to camera, microphone, and LiDAR requires explicit user permission
- Exported files are protected by iOS file system permissions

## Data Sharing and Transfer

### No Third-Party Sharing

SpecimenPro **does not share, sell, or transmit your data to any third parties**. Your data remains entirely under your control.

### User-Initiated Sharing

You may choose to share your data through:

- **Export Function**: Exporting database files (ZIP or .db format) to share with colleagues or for backup
- **Share Sheet**: Using iOS's native share functionality to send exported files via email, AirDrop, or other apps
- **iCloud**: If you choose to save exported files to iCloud Drive (user-initiated only)

When you export or share data, you are responsible for ensuring compliance with any applicable data protection regulations.

## Permissions

SpecimenPro requests the following permissions:

- **Camera**: To capture photos of specimens and scan QR codes
- **Microphone**: To record voice notes
- **Photo Library**: To save and access photos
- **File System**: To import/export database files

You can revoke these permissions at any time through your device's Settings app.

## Data Retention

- Data is retained on your device until you explicitly delete it
- Deleting a collection, object, photo, or voice note permanently removes it from the database
- Automatic backups are created before database imports
- You can manually export data for long-term archival

## Your Rights and Choices

You have the following rights regarding your data:

1. **Access**: View all your data within the app
2. **Export**: Export your entire database or individual collections at any time
3. **Delete**: Delete individual items, collections, or the entire database
4. **Modify**: Edit and update any information you've entered
5. **Backup**: Create backups through the export function
6. **Import**: Restore data from previously exported files

## Children's Privacy

SpecimenPro complies with the Children's Online Privacy Protection Act (COPPA) and is rated by Apple to be 4+ years old. The app is designed for professional and educational use by researchers, curators, and students. 

## Changes to This Privacy Policy

We may update this Privacy Policy from time to time. Changes will be reflected in the "Last Updated" date at the top of this policy. Continued use of the app after changes constitutes acceptance of the updated policy.

## Data Protection Compliance

### GDPR Compliance (European Users)

If you are located in the European Economic Area (EEA), you have additional rights under the General Data Protection Regulation (GDPR):

- **Right to Access**: Request a copy of your data (available through export function)
- **Right to Rectification**: Correct inaccurate data (available through edit functions)
- **Right to Erasure**: Delete your data (available through delete functions)
- **Right to Data Portability**: Export your data in a structured format (available through export function)
- **Right to Object**: Object to data processing (you control all data processing)

### CCPA Compliance (California Users)

California residents have the right to:

- Know what personal information is collected
- Know whether personal information is sold or disclosed (SpecimenPro does not collect or sell your data)
- Access their personal information (available through the app)
- Request deletion of personal information (available through delete functions)

## Third-Party Services

SpecimenPro does not integrate with any third-party analytics, advertising, or tracking services. The app communicates with external servers only for the following purposes:

### Events Server

- **Purpose**: To download virtual event information (mineral shows, fossil fairs, etc.)
- **Server**: GitHub Pages (aaroncelestian.github.io/specimenpro-events)
- **Data Downloaded**: Event details, specimen information, QR codes, and event schedules
- **Data Sent**: None - the app only downloads event information, it does not upload any of your data
- **Caching**: Event data is cached locally for 1 hour to minimize server requests
- **Privacy**: Your event progress and participation are stored only on your device and never transmitted to our servers

### Apple StoreKit

- **Purpose**: To process in-app purchases and verify purchase status for the Full version upgrade
- **Data Shared**: Purchase verification requests are sent to Apple's servers through the StoreKit framework
- **Apple's Privacy**: All payment processing and purchase records are governed by Apple's Privacy Policy
- **No Personal Data**: We do not receive or have access to your payment information, Apple ID, or other personal details from Apple

## Contact Information

If you have questions or concerns about this Privacy Policy or your data, please contact:

**Developer**: Aaron Celestian  
**Email**: [Your contact email]  
**App**: SpecimenPro

## Technical Details

### Data Types Stored

- **Collections**: Name, type, date, collector, custom fields, custom photo types
- **Objects**: Number, specimen ID, metadata (JSON), tags (JSON)
- **Photos**: Image data (BLOB), thumbnails (BLOB), photo type, creation date
- **Voice Notes**: Audio data (BLOB), duration, title, creation date
- **Database Schema**: Version 5 (SQLite)
- **License Information** (stored in UserDefaults, not in database):
  - Install date (for grandfathering)
  - Purchase status flag (boolean)
  - Grandfathered status flag (boolean)
- **Event Progress** (stored in UserDefaults, not in database):
  - Event participation progress
  - Collected specimens per event
  - Cached event data (expires after 1 hour)

### Data Format

- Database: SQLite 3
- Export Format: ZIP archive containing SQLite database and README
- Image Format: JPEG/PNG (compressed)
- Audio Format: M4A/WAV

### Data Encryption

- iOS file system encryption (when device is locked)
- App sandbox security
- No additional encryption layer (data is local only)

## Disclaimer

SpecimenPro is provided "as is" for specimen data management. Users are responsible for:

- Maintaining their own backups
- Ensuring compliance with institutional data policies
- Protecting sensitive or confidential specimen information
- Following applicable laws and regulations when collecting and sharing data

## Open Source

SpecimenPro may use open-source components. All open-source licenses are respected and acknowledged.

---

**By using SpecimenPro, you acknowledge that you have read and understood this Privacy Policy and agree to its terms.**

For the most current version of this Privacy Policy, please check the app documentation or contact the developer.

# DynFOTech-SAF-T (NO)

### 🇳🇴 Microsoft Dynamics 365 Finance and Operations – SAF-T (Norway) Custom Configuration

This repository contains community-ready configurations for the **Standard Audit File (SAF-T)** in Norway, fully compatible with Microsoft Dynamics 365 Finance & Operations (D365FO).

---

## 📦 Included Files

| Folder | Description |
|---------|-------------|
| **DataModel** | Contains the latest plain Microsoft Standard Audit File (SAF-T) data model. |
| **ModelMapping** | Contains the latest plain Microsoft SAF-T Financial Data Model mapping configuration. |
| **Format** | Contains the customized Norwegian SAF-T format with English and Norwegian labels to optimize setup performance. |

---

## ⚠️ Version Compatibility

All configurations in this repository must be used in **the same version** to ensure compatibility between the data model, mapping, and format.

Example of a consistent version set:
- **Data model:** Standard Audit File (SAF-T) *(190)*
- **Model mapping:** SAF-T Financial data model mapping *(190.146)*
- **Format:** SAF-T Format (NO)-DFT *(190.179)*

The **Data model** acts as an **enabler** for the **Format** — meaning:
- You **must import** `Standard Audit File (SAF-T) (190)` **first**,  
- and then import `SAF-T Format (NO)-DFT (190.179)`.

Version `190` represents the **format version** and must match across all configurations.

---

## 🧰 Installation Guide

1. **Import Standard Files**
   - Import the following Microsoft standard configurations:
     - `Standard Audit File (SAF-T)`
     - `SAF-T Financial data model mapping`
   - If you already have newer versions of these files, you can skip this step.

2. **Prepare Existing Setup**
   - Open **Application specific parameters setup**.
   - Export your existing mapping table.

3. **Import Custom SAF-T Format (NO)**
   - Import the customized configuration from the `Format` folder.
   - Verify that the imported version is the **latest**.
   - Delete any older versions of the configuration.

4. **Reopen Application Specific Parameters**
   - The setup form will now open faster due to minimized labels and configuration size.
   - Import your saved mapping table again if needed.
   - Replace the mapping table with company-specific mappings if applicable.

---

## 🧩 Compatibility
- **Dynamics 365 Finance and Operations (D365FO)**
- Supports the latest Microsoft SAF-T configurations and data model versions.

---

## 🆓 License
This configuration is **open and free** for the Microsoft community to download and use.

---

## 🤝 Credits
Created and maintained by **[Alireza Eshaghzadeh](https://github.com/Alireza-Eshaghzadeh)**  
Microsoft MVP | Dynamics 365 Finance & Operations | Knowit Insight Business Solutions
https://dynfotech.com/
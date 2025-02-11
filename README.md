# Microsoft Activation Scripts (MAS)


Microsoft Activation Scripts (MAS) is an open-source tool that enables activation of Windows and Office products using multiple methods. It features HWID, Ohook, KMS38, and Online KMS activation methods along with advanced troubleshooting techniques.

> **Disclaimer:** This tool is provided for educational and testing purposes only. Use it at your own risk. The developers do not endorse any illegal activities. Please ensure you comply with your software licensing agreements and local laws.

---

## Table of Contents

<div align="center">
  [![Introduction](https://img.shields.io/badge/Introduction-blue?style=flat-square)](#introduction)
  [![Features](https://img.shields.io/badge/Features-blue?style=flat-square)](#features)
  [![Installation](https://img.shields.io/badge/Installation-blue?style=flat-square)](#installation)
  [![Usage](https://img.shields.io/badge/Usage-blue?style=flat-square)](#usage)
  [![Activation Summary](https://img.shields.io/badge/Activation_Summary-blue?style=flat-square)](#activation-methods-summary)
  [![Troubleshooting](https://img.shields.io/badge/Troubleshooting-blue?style=flat-square)](#troubleshooting)
 
</div>

---


## Introduction

Microsoft Activation Scripts (MAS) is an all-in-one tool designed to simplify the activation process for Microsoft Windows and Office products. With support for various activation methods, MAS provides a user-friendly and efficient solution for system activation.

---

## Features

- **Multiple Activation Methods:**  
  - **HWID Activation:** Permanently activates Windows 10/11.
  - **Ohook Activation:** Permanently activates Office.
  - **KMS38 Activation:** Activates Windows 10/11/Server until the year 2038.
  - **Online KMS Activation:** Activates Windows and Office for 180 days, with an automatic renewal task for lifetime activation.
- **Easy to Use:** Run a single PowerShell command to initiate the activation process.
- **Advanced Troubleshooting:** Built-in troubleshooting steps to help resolve common activation issues.
- **Open-Source:** Fully transparent codebase allowing for community review and contributions.

---

## Installation

### Prerequisites

<div align="center">
  <table>
    <tr>
      <td align="center" style="padding: 10px;">
        <img src="https://img.shields.io/badge/Windows-10%2F11%2FServer-blue?style=for-the-badge" alt="Windows">
        <br>
        <strong>Windows 10/11/Server</strong>
      </td>
      <td align="center" style="padding: 10px;">
        <img src="https://img.shields.io/badge/PowerShell-Required-blue?style=for-the-badge" alt="PowerShell">
        <br>
        <strong>PowerShell</strong><br>
        (Run as Administrator)
      </td>
      <td align="center" style="padding: 10px;">
        <img src="https://img.shields.io/badge/Internet-Required-blue?style=for-the-badge" alt="Internet">
        <br>
        <strong>Internet Connection</strong><br>
        (For Online KMS)
      </td>
    </tr>
  </table>
</div>

### Steps

1. **Open PowerShell as Administrator.**

2. **Execute the Activation Scripts:**

   - For **Windows Activation**, run:
     ```powershell
     irm https://get.activated.win | iex
     ```

   - For **Office Activation**, run:
     ```powershell
     irm https://massgrave.dev/get | iex
     ```

*Note:* The commands above use `irm` (Invoke-RestMethod) to fetch and execute the activation scripts. Always ensure you trust the source before executing remote scripts.

---

## Usage

After executing the scripts, MAS will automatically detect your system's configuration and apply the appropriate activation method based on your installed product.

1. **Automatic Detection:**  
   The script identifies whether your system requires Windows or Office activation.

2. **Activation Process:**  
   Depending on the product, one of the following methods is applied:
   - **HWID Activation:** Activates Windows 10/11 permanently.
   - **Ohook Activation:** Activates Office permanently.
   - **KMS38 Activation:** Activates Windows 10/11/Server until 2038.
   - **Online KMS Activation:** Activates Windows/Office for 180 days with an automatic renewal task for lifetime activation.

3. **Confirmation:**  
   A confirmation message will appear in the PowerShell window once activation is successful.

---

## Activation Methods Summary

| Activation Type  | Supported Product            | Activation Period                  | Internet Required? |
| ---------------- | ---------------------------- | ---------------------------------- | ------------------ |
| **HWID**         | Windows 10-11                | Permanent                          | Yes                |
| **Ohook**        | Office                       | Permanent                          | No                 |
| **KMS38**        | Windows 10-11-Server         | Till the Year 2038                 | No                 |
| **Online KMS**   | Windows / Office             | 180 Days (Lifetime with Renewal)   | Yes                |

---

## Troubleshooting

If you encounter issues during activation, consider the following steps:

- **Verify Internet Connection:**  
  Ensure that your device is connected to the internet if using Online KMS activation.

- **Run as Administrator:**  
  Always run PowerShell as an Administrator to avoid permission issues.

- **Disable Security Software:**  
  Temporarily disable antivirus or firewall software that might block the script.

- **Review Output Logs:**  
  Check the PowerShell output for error messages or warnings that can guide further troubleshooting.

---

## Advanced Topics

- **Custom Activation Methods:**  
  Developers can extend MAS by adding new activation methods. The code is well-commented for easy customization.

- **Task Scheduler Integration:**  
  For Online KMS activation, you can set up a scheduled task to automatically renew activation every 180 days.

- **Script Debugging:**  
  For those interested in the inner workings, the source code is available for review and debugging.

---



*Happy Activating!*



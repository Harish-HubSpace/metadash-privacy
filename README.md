# 🚀 MetaDash - Salesforce Custom Field Dependency & Diff Scanner

MetaDash is a lightweight browser utility engineered to help Salesforce Developers and Release Engineers analyze custom field dependencies and check cross-environment deployment schema alignment in seconds.

---

## 🛠️ How to Use MetaDash

### Feature 1: Custom Field Usage Analyzer (Apex Scanner)
1. Log into your Salesforce Org and navigate to **Setup**.
2. Go to **Object Manager** and click on any object (e.g., *Account* or *Custom_Object__c*).
3. Click the **MetaDash** extension icon in your Chrome toolbar.
4. Hit **Scan Code Dependencies**. 
   * *MetaDash will instantly run a parallel batch scan to show you which custom fields are referenced in your Apex classes, and which ones are completely safe to prune.*

### Feature 2: Cross-Environment Diff Checker
1. Open a separate browser tab and log into your **Target Environment** (e.g., Production or your UAT Sandbox).
2. Return to your original Salesforce Setup tab where you have MetaDash open.
3. Open the MetaDash popup window and paste the base URL of your target environment into the input box (e.g., `https://mycompany--uat.sandbox.lightning.force.com`).
4. Click **Compare Object Fields**.
   * *The discrepancy matrix will instantly call out missing deployments or data type configuration drift across your environments.*

---

## 🔒 Security & Privacy
MetaDash operates on a 100% read-only, local browser sandbox architecture. It reads your active session identifier (`sid`) locally via Chrome cookies to safely call the Salesforce Tooling API. **Your credentials and metadata never leave your browser.**

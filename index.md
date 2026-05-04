# Privacy Policy for Extreme Note

**Effective Date:** May 2026

Thank you for using Extreme Note! We are committed to protecting your privacy. This Privacy Policy explains what information we collect, how we use it, and how we protect it.

## 1. Local Storage Only
Extreme Note is designed to be a local-first application. All your notes, spreadsheets, tags, settings, and captured data are stored **locally** on your device using your browser's local storage (`chrome.storage.local`). 
- We do not run any central servers to store your notes.
- We do not transmit your notes to any third-party analytics or tracking services.

## 2. Permissions We Request

To provide its core functionality, Extreme Note requests the following permissions:
- **`storage`**: Required to save your notes, settings, and captures locally on your device.
- **`activeTab` / `scripting`**: Required *only* when you explicitly use the "Capture from page" button. It allows the extension to read the text you have highlighted on the current webpage or capture its URL and description.
- **`contextMenus`**: Allows capturing content via right-click menus.
- **`sidePanel`**: Allows the extension to run natively within Chrome's Side Panel interface.
- **`identity`**: Required *only* when you click "Export to Google Doc", "Export to Google Sheet", "Save to Google Drive", or "Open Google". It is used exclusively to obtain an OAuth token from your own Google account so the extension can talk to Google APIs on your behalf. No identity data is sent anywhere else.

## 3. Third-Party Services and API Usage

### Google Drive, Google Docs, and Google Sheets
Extreme Note includes optional features to export and read your notes/spreadsheets in your own Google account.
- The extension will **never** access your Google account until you explicitly click one of the Google buttons ("Export to Google Doc", "Export to Google Sheet", "Save to Google Drive (.md)", or "Open Google").
- The requested scopes are:
  - `https://www.googleapis.com/auth/documents` — create new Google Docs and read the body of Docs you opened via the extension.
  - `https://www.googleapis.com/auth/spreadsheets` — create new Google Sheets and read sheets you opened via the extension.
  - `https://www.googleapis.com/auth/drive.file` — per-file access. The extension can only see files it created itself or files you explicitly opened with it. It cannot see, list, modify, or delete any other files in your Drive.
- The "Open Google" button lists only files visible under the `drive.file` per-file scope (i.e. files this extension created or you previously opened with it). The content of the file you click is fetched once and loaded into a local tab; it is not sent anywhere else.
- The use of information received from Google APIs will adhere to the [Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy), including the Limited Use requirements.

### MyMemory Translation API
Extreme Note includes a translation feature that utilizes the free, public MyMemory Translation API (`api.mymemory.translated.net`).
- Only the specific text you highlight and choose to translate is sent to this service.
- No personal identifiers, account data, or entire notes are sent.

## 4. Data Sharing and Selling
We **do not** sell, rent, or trade any of your personal information or note content to third parties. We do not use your data for advertising purposes.

## 5. Changes to This Privacy Policy
We may update this Privacy Policy from time to time. Any changes will be reflected with an updated "Effective Date" at the top of this document.

## 6. Contact Us
If you have any questions or concerns about this Privacy Policy or how your data is handled, please contact the developer via the Chrome Web Store support page.

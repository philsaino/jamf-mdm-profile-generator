# Jamf MDM Profile Generator

This repository contains a simple, single-page web application to generate Apple MDM (Mobile Device Management) enrollment profiles (`.mobileconfig` files) for use with Jamf Pro.

## What It Does

- Provides a clean web form to input:
  - **MDM Invitation ID** — the enrollment challenge token.
  - **Jamf URL** — your Jamf Pro server URL.

- Automatically generates a valid UUID for the profile on each generation.

- Dynamically crafts a `.mobileconfig` XML configuration profile compatible with Jamf’s MDM enrollment.

- Allows the user to download the generated `.mobileconfig` file directly from the browser without any server-side code or installation.

## Why This Is Useful

- Enables creating custom Jamf enrollment profiles easily and quickly from any device with a modern web browser.

- Does NOT require any backend or local script execution; the entire logic runs client-side with JavaScript.

- Perfectly suited to be hosted on GitHub Pages or similar static site hosting services.

## Usage

1. Open the page in your browser at the hosted URL:  
   [https://philsaino.github.io/jamf-mdm-profile-generator/](https://philsaino.github.io/jamf-mdm-profile-generator/)

2. Fill in the MDM Invitation ID and Jamf URL fields.

3. Click "Generate Profile" to download the `.mobileconfig` file.

4. Use the downloaded file to enroll your macOS device into Jamf MDM.

## Tech Stack

- HTML5 and CSS3 for layout and styling.

- JavaScript (vanilla) for UUID generation and file creation.

## Customization

You can easily modify:

- The styling in `index.html` to match your branding.

- The XML template to adjust profile parameters.

## License

Open source under MIT License.

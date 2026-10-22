# 📱 QRift — Offline QR Text Transfer 💻

**Bridge devices. Not servers.**

QRift is a lightweight, privacy-focused tool designed to transfer text, code snippets, URLs, and clipboard content between devices using QR codes.

Generate a QR code on one device and scan it with another. No account, no cloud sync, and no backend required for the core transfer workflow. Everything happens blazing fast, at the speed of 'sight' ☺️.

<p align="center">
  <strong>Scan. Transfer. Done.</strong>
</p>

<p align="center">
  <a href="https://opensource.org/licenses/MIT">
    <img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="MIT License">
  </a>
  <img src="https://img.shields.io/badge/Offline-Capable-00bcd4.svg" alt="Offline capable">
  <a href="http://makeapullrequest.com">
    <img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg" alt="PRs Welcome">
  </a>
</p>

<p align="center">
  <strong><a href="#">🚀 Live Demo — Coming Soon</a></strong>
</p>

---

##  Features

- ** Frictionless Transfer:** Generate QR codes instantly as you type or paste text, URLs, and code snippets.
- ** Two-Way Workflow:** Use the Send tab to generate QR codes and the Receive tab to scan them.
- ** Quick Copy:** Copy scanned text directly to your clipboard.
- ** Open Links:** Recognizes URLs and lets you open them directly.
- ** Recent History:** Keeps your last 10 scans during the current session, with options to copy text or open links.
- ** Privacy-Focused:** No accounts, cloud sync, or backend required for the core workflow.
- ** Offline-Capable:** Uses local QR libraries, so the app can work without an internet connection when all required files are available.
- ** Developer-Friendly:** Handy for transferring debugging output, configuration strings, code snippets, and other development notes.
- ** Cross-Device:** Transfer information between Android phones, laptops, and other devices with a compatible QR scanner.
- ** Lightweight:** A simple browser-based utility with no sign-up required.

##  Try QRift

### Option 1: Use the Live Demo

**Live Demo:** Coming soon!

The hosted version can be opened directly without installing anything. An internet connection is needed to load the site for the first time unless its files are already cached.

For camera scanning, use the HTTPS version of the site and allow camera access when prompted.

### Option 2: Download and Run Offline

Want to try QRift without installing additional software?

1. Open the QRift GitHub repository.
2. Click the green **Code** button.
3. Select **Download ZIP**.
4. Extract the downloaded ZIP file.
5. Open the extracted project folder.
6. Open `qr.html` in your browser.

Make sure these files remain in their expected locations:

- `qr.html`
- `qrcode.min.js`
- `html5-qrcode.min.js`
- `assets/icon.png`

QR generation may work directly from the local HTML file. Camera scanning depends on browser security restrictions and may not work when opened this way.

### Option 3: Clone the Repository with Git

If Git is installed, download the source code with:

```bash
git clone https://github.com/YOUR-USERNAME/qrift.git
cd qrift
```

Open `qr.html` in your browser to try the app. No package installation is required for the current standalone version.

---

## How It Works

1. Open QRift on your sending device.
2. Select the **Send** tab.
3. Type or paste the text you want to transfer.
4. QRift generates the QR code automatically.
5. On the receiving device, open a compatible QR scanner or QRift's **Receive** tab.
6. Scan the code to retrieve the text.

For example, generate a QR code on your Android phone and scan it using your laptop camera to transfer a URL or code snippet.

In the Receive tab, QRift displays the latest scan, copies the decoded text to your clipboard, and lets you open detected URLs. Recent scans are listed for quick access during the current session.

**Note:** The receiving device needs a compatible QR scanner. Camera access must be supported and permitted by the browser when using QRift's built-in scanner.

## Offline Usage

QRift includes local references to its QR generation and scanning libraries rather than loading them from a CDN.

For offline use:

- Keep `qrcode.min.js` and `html5-qrcode.min.js` alongside `qr.html`.
- Download the project files before disconnecting from the internet.
- Generate QR codes locally without relying on a remote service.
- Test camera scanning separately, since browser permissions and local-file restrictions can affect it.

The GitHub Pages demo is hosted online and requires an initial connection to load unless the necessary files are already cached. Offline access to the hosted version is not guaranteed.

## 🔒 Privacy and Security

QRift is designed for local text transfer without accounts or cloud synchronization.

- No account or sign-up required.
- No backend required for the core transfer workflow.
- QR generation and text handling happen in the browser.
- Recent scan history is held in memory and is not persisted across page reloads.
- Anyone who can see a QR code may be able to scan its contents.

**Security note:** Avoid encoding passwords, authentication tokens, private keys, or other sensitive information into QR codes that could be photographed or scanned by others.

## 🛠️ Built With

- **HTML5** — Page structure
- **CSS3** — Styling and responsive layout
- **JavaScript** — QR generation, scanning, and text handling
- **[QRCode.js](https://github.com/davidshimjs/qrcodejs)** — QR code generation
- **[html5-qrcode](https://github.com/mebjas/html5-qrcode)** — Camera-based QR scanning

##  Roadmap

- [ ] Publish the first working release.
- [ ] Deploy the live demo using GitHub Pages.
- [ ] Test QR generation with longer text payloads.
- [ ] Verify offline functionality.
- [ ] Test scanning across Android phones and desktop browsers.
- [ ] Improve handling of large QR payloads.
- [ ] Add screenshots and usage examples.
- [ ] Improve accessibility and mobile usability.

## 🤝 Contributing

Contributions, bug reports, and feature suggestions are welcome!

1. Fork the repository.
2. Create a branch for your changes.
3. Make and test your improvements.
4. Submit a pull request describing your changes.

For significant changes, please open an issue first to discuss the proposal.

## 📄 License

This project is intended to use the MIT License.

See the [LICENSE](LICENSE) file for details.

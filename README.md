# 📄 Legal Contracts & eSign Boilerplate

A modern Next.js 15 boilerplate built with Tailwind CSS, designed for freelancers, legal professionals, and SaaS founders who need to manage, send, and sign legal documents digitally.

---

## ✨ Features

- 🧾 Create and edit legal contracts using a rich text editor
- ✍️ Capture eSignatures using a canvas-based signature pad
- 📄 Export contracts to downloadable PDFs
- 📬 Send contract invites via email
- 👤 Basic authentication (placeholder – easily extend with Clerk, NextAuth, etc.)
- 🛠️ Extendable with Stripe for monetization, roles, versioning, etc.

---

## 🧱 Tech Stack

- **Framework:** Next.js 15 (App Router)
- **Styling:** Tailwind CSS + HeroUI
- **PDF Export:** @react-pdf/renderer + html2canvas
- **Signature Capture:** react-signature-canvas
- **Auth Ready:** Integrate Clerk or NextAuth easily
- **Email Notifications:** Brevo, Resend, or SendGrid compatible

---

## 📁 Project Structure

<pre lang="markdown"> ```bash legal-esign-boilerplate/ ├── app/ │ ├── layout.jsx # Root layout │ ├── globals.css # Tailwind base styles │ │ ├── dashboard/ │ │ └── page.jsx # User's contract dashboard │ │ ├── contracts/ │ │ └── [contractId]/ │ │ ├── page.jsx # View contract & sign │ │ ├── edit.jsx # Edit contract │ │ └── actions.js # Server actions: signContract, saveSignature │ │ └── auth/ │ ├── login.jsx # Login page │ └── signup.jsx # Signup page │ ├── components/ # Shared UI components │ ├── Navbar.jsx │ ├── ContractList.jsx │ ├── ContractEditor.jsx │ ├── SignaturePad.jsx │ └── PdfPreview.jsx │ ├── lib/ # Utility functions │ ├── pdfUtils.js │ ├── emailUtils.js │ └── signatureUtils.js │ ├── public/ # Static assets (e.g. logo, icons) ├── .gitignore ├── README.md ├── tailwind.config.js ├── postcss.config.js ├── package.json └── next.config.js ``` </pre>


## 🚀 Getting Started

### 1. Clone the Repo

git clone https://github.com/yourusername/legal-esign-boilerplate.git
cd legal-esign-boilerplate

### 2.  Install the dependencies

npm install

### 3.  Install the dependencies

npm run dev
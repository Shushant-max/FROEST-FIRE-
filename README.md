# Forest Fire Detection

A professional forest fire detection web app with a real-world AWS Rekognition backend.

## Features

- modern responsive landing page layout
- image upload and live preview
- local Express backend with AWS Rekognition integration
- detection result, confidence, and risk level display

## Files

- `index.html` — main UI structure
- `styles.css` — polished visual design
- `script.js` — frontend upload and analysis workflow
- `server.js` — Node.js backend endpoint for Rekognition requests
- `package.json` — dependencies and run script
- `.env.example` — environment variables for AWS credentials

## Setup

1. Copy `.env.example` to `.env`.
2. Fill in your AWS credentials and preferred region.
3. Run `npm install`.
4. Run `npm start`.
5. Open `http://localhost:3000/index.html` in your browser.

## AWS Rekognition integration

The backend receives an image upload, sends it to AWS Rekognition using `detectLabels`, and determines if fire or smoke-related labels are present.

### Environment variables

- `AWS_ACCESS_KEY_ID`
- `AWS_SECRET_ACCESS_KEY`
- `AWS_REGION`
- `PORT` (optional, default `3000`)

### Security note

Never store AWS credentials in client-side code. This app keeps credential handling on the server.

## Running locally

Open the browser at `http://localhost:3000/index.html`, upload a forest image, and click **Analyze with Rekognition**.

## Notes

- If the backend is unavailable, the frontend falls back to a local simulation mode.
- Update `server.js` to refine detection rules and label scoring for production use.
"# FROEST-FIRE-" 

1. Import Workflow
n8n → Workflows → Import from File → Select `Niveshaay_Workflow_Clean.json`
2. Set Up Credentials (No hardcoding)
Create 3 credentials in n8n:
Service	Type	Where to set
Gemini	Header Auth	`https://generativelanguage.googleapis.com/v1beta/models/gemini-3.5-flash:generateContent?key=YOUR_KEY` - Replace `{{$env.GEMINI_API_KEY}}` or add Header Auth credential
Cofferdock	Header Auth	Header `x-api-key: YOUR_COFFERDOCK_KEY`, `Content-Type: application/json`
Evolution WhatsApp	Header Auth	Header `apikey: YOUR_EVO_APIKEY`, Instance `n8n_whatsapp` must be connected (scan QR at `/instance/connectionState/n8n_whatsapp`)
> For submission: Keys are removed.
3. Run
Activate workflow
Open Form URL (from Form Trigger node)
Enter: `Company Name: E2E Networks Limited` + `Result PDF URL: https://www.bseindia.com/xml-data/corpfiling/AttachLive/...pdf`
Submit → Check WhatsApp number `91 83029 61064` for image. (Open n8n → Your workflow → Send To Whatsapp node: Replace with your number in international format without +)
---
Author: Akshat Bhutra

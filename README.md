# MarkerTool
This toolset is designed to detect silent intervals in audio files and add markers to the Premiere Pro timeline based on those intervals.

# **Silent Detection and Adobe Premiere Pro Marker Tool**

This guide walks you through creating a **silent detection tool** using Python and building an **Adobe Premiere Pro extension** to automatically add silence markers to your sequences.

---

## **Step-by-Step Guide**

### **Step 1: Create a Python Script to Detect Silence**

1. **Setup Python Environment**

   - Ensure Python 3.x is installed on your system.
   - Install the required library `pydub`:
     ```bash
     pip install pydub
     ```

2. **Write the Silent Detection Script**

   Create a Python script (`detect_silence.py`) with the following content:
   Contact hieund.hi.tech@gmail.com to access `detect_silence.py`

### **Step 2: Build Adobe Premiere Pro Extension**
## Self-Sign the Extension

To sign the extension, you will use **Adobe's ZXPSignCmd** tool. Follow these steps:

```bash
ZXPSignCmd -selfSignedCert US California "hieu95" "hieu95cert" "password" certificate.p12 -locality "City" -orgUnit "IT Department" -email "youremail@example.com" -validityDays 3650

ZXPSignCmd -sign SilentMarkers ./signed/SilentMarkers.zxp ./cert.p12 password

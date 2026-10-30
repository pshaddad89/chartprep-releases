# ChartPrep: try-out version (downloads)

ChartPrep is a prototype pre-visit tool for internal medicine. It reads a patient's chart and
scanned outside records and gives you a one-page pre-visit brief, plus a small "chart helper"
window where you can search the chart and ask questions. Every answer points to the page it
came from.

**This try-out contains made-up patients only: six samples, plus the fake patients in Oracle
Health's public test sandbox. Never type or paste real patient information into it.**

## Download

Get the newest **ChartPrep-Setup-x.x.exe** from the
[Releases page](https://github.com/pshaddad89/chartprep-releases/releases/latest)
(under "Assets").

You need a Windows 10 or 11 computer, an internet connection, and the access key you were sent
separately.

## Install

1. Double-click the downloaded `ChartPrep-Setup-x.x.exe` and follow the steps. No administrator
   password is needed.
2. Windows will probably show **"Windows protected your PC"** (unknown publisher). The installer
   isn't digitally signed yet. Click **More info**, then **Run anyway**. If your browser warns
   that the file is "not commonly downloaded", choose **Keep**. If your antivirus blocks it, tell
   the person who sent you the link; please don't turn your antivirus off.
3. Leave "Start ChartPrep now" ticked and click Finish. Later, find it in the Start menu.

## First run

Paste the access key you were sent and click **Save key**. It's stored, encrypted, only on your
computer. You can skip this: the sample patients, searching them and reading their briefs work
without it. Questions, briefs for sandbox patients and reading their scanned documents need it.

## Using it

- Click a patient to open the chart helper. Search with words like *metformin*, or ask a question
  ending with "?".
- Click a **source** link to see the original page in the bottom half of the window, with the
  quoted words to look for. **Full screen** enlarges it; **Esc** closes it.
- **Brief** opens the one-page pre-visit brief in your browser.
- The **Search the Oracle sandbox** tab finds other test patients by MRN, sandbox ID or last name.
  They load live, and the first time one is opened the AI reads its scanned documents (a few
  cents a page) and writes the brief (about 5 cents).
- Opening the six sample patients is free. Each question costs a few cents on your key; the launcher shows the
  running total.
- **Send feedback** saves a text file in *Documents\ChartPrep feedback* for you to email back.

## Uninstall

Settings > Apps > Installed apps > **ChartPrep (try-out)** > Uninstall. This also removes the
saved key.

## Checking the download (optional)

Each release lists the file's SHA-256 checksum. In PowerShell:
`Get-FileHash .\ChartPrep-Setup-0.6.exe` should show the same value.

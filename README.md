# 1. Source Code Review Using Corgea
### Installation
```
1. Create account on : https://corgea.com/
2. Login in web & and save the login token corgea login: ebbc1ce1-b945-4bd8-9eda-3d16e2ca4a2e
```
### Execution

```
1. Login to the  https://corgea.com/
2. Open cms & execute: corgea login ebbc1ce1-b945-4bd8-9eda-3d16e2ca4a2e
3. Go to your project folder and execute: corgea scan
4. Check https://www.corgea.app/scans/ for output.
```
### OUTPUT:
```
Scan has started with ID: de69d6af-14c1-44f7-8c2a-797409a4d0ef.

You can view it populate at the link:
https://www.corgea.app/project/Source Code?scan_id=de69d6af-14c1-44f7-8c2a-797409a4d0ef

Your scan will continue securely in the Corgea cloud.
You can safely exit the process now if you prefer not to wait for it to complete.

╭────────────────────────────────────────────╮
│                                            │
│   🎉🎉 Scan Completed Successfully! 🎉🎉   │
│                                            │
╰────────────────────────────────────────────╯

Scan Results:-

Classification       | Count
-------------------- |
CR                   | 3
HI                   | 3
ME                   | 0
LO                   | 0
-------------------- |
Total                | 6


You can view the scan results at the following link:
https://www.corgea.app/project

```
# 2. Secure Source Code Review Using Auditor
### Installation
```
1. git clone https://github.com/TheAuditorTool/Auditor
2. cd Auditor
3. pip install -e .
```
### Execution

```
1. cd ~/your-project
2. aud init && aud full
```
### OUTPUT:
```
============================================================
[COMPLETE] AUDIT SUITE EXECUTION COMPLETE
============================================================
[SAVED] Full pipeline log saved to: .pf\pipeline.log
============================================================
AUDIT FINAL STATUS
============================================================
STATUS: [CRITICAL] - Audit complete. Found 3 critical vulnerabilities.
Immediate action required - deployment should be blocked.
Findings breakdown:
  - Critical: 3
  - High: 62
  - Medium: 38
  - Low: 2
Review the chunked data in .pf/readthis/ for complete findings.
```
```
 =================================================================
|OUTPUT FILE LOCATION :->your-project/.pf/readthis/patterns.json  |
 =================================================================
```
# 3. Secure Source Code Review Using Semgrep
### Installation
```
1. pip install semgrep 
2. semgrep --version    
```
### Execution

```
1. cd ~/your-project
2. semgrep --config auto .
3. semgrep --config auto . --json
```

### OUTPUT: semgrep-results.json
```
 =================================================================
|OUTPUT FILE LOCATION :->your-project/semgrep-results.json |
 =================================================================
```

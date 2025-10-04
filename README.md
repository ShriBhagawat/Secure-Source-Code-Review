# Secure Source Code Review Using Auditor
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
 ===========================================================================
|OUTPUT FILE LOCATION :->your-project/.pf/readthis/patterns.json  |
 ===========================================================================
```

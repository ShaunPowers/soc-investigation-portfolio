# <Report title> (training exercise)

**Type:** training exercise | simulated incident | personal lab project
**Platform or lab:** <TryHackMe room name / LetsDefend case / Splunk home lab>
**Date investigated:** YYYY-MM-DD
**Time spent:** <hours>

> This write-up describes my own investigation of a simulated scenario. No real organisation or real victim data is involved. Platform answers and flags are not reproduced.

## 1. Objective and scenario

What the alert or task said. What question I had to answer. What a correct outcome would look like.

## 2. Tools and data sources

| Tool | Used for |
|------|----------|
| e.g. Splunk Enterprise | searching Windows Security logs |
| e.g. Wireshark | reading the packet capture |

Data: which log sources, which index or file, which time window.

## 3. Evidence and indicators

Bullet list of what was found, each with where it came from (event ID, log line, packet number, URL, hash). Indicators of compromise in a table:

| Indicator | Type | Where seen | Note |
|-----------|------|------------|------|
| | IP / domain / hash / user / file | | |

## 4. Queries and commands used

Exactly as run, in order. One code block each, with a one-line note on what it was for.

```spl
index=main sourcetype=WinEventLog:Security EventCode=4625 | stats count by Account_Name, Source_Network_Address
```

## 5. Investigation reasoning

Step by step: what I looked at first, why, what it showed, what I checked next. Where I was wrong and corrected course.

## 6. MITRE ATT&CK techniques

| Tactic | Technique | ID | Evidence that supports it |
|--------|-----------|----|---------------------------|
| | | T#### | |

## 7. Verdict

**True positive / False positive / Benign true positive**, and the one or two facts that decide it.

## 8. Severity and escalation

Severity (low / medium / high / critical) and why. Escalate to Tier 2, close, or monitor. What I would want from the next tier.

## 9. Incident summary

Five to eight plain-English sentences a manager could read, built on the Five Ws in this order: Who (user and account), What (the exact sequence of events), When (start and end times), Where (device, IP, URL or site), Why (the reasoning behind the verdict). Then what should be done.

## Lessons

What I learned, what I would check faster next time.

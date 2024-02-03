---
title: "AMUQP"
date: 2023-06-26T22:21:34+05:30
draft: true
---

## What is AMUQP?
AMUQP is a bloat-free, lightning fast platform for downloading previous-year question papers of AMU's engineering exams. It offers searching by:* Name
- Session
- Department
- Exam Type (mid/end)
- Subject Code

It uses *fuzzy-searching* (approximate searching) for ranking results. 

## TODO
- [X] Web interface
- [X] Google Form for paper submission with automatic renaming of uploaded file based on user-provided metadata (session, branch, subject code, etc)
- [X] A Google App Script (GAS) triggered on every form submit that fetches the newly added data in the Google Sheet (connected to the Google Form) and sends a POST request to update the DB.
- [ ] Check for duplicate papers.




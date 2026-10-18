---
title: "SIGPAE: Syllabus Management System"
date: 2017-03-01
lastModifiedAt: 2018-10-14
description: Django web application for transcription of course syllabi
path: /blog/sigpae
project: 'SIGPAE'
---

As part of our **Software Engineering** course in the _Universidad Simón Bolívar_, eight (8) of us, as Team "Zenpy" (notice me), developed, during five (5) weeks, a nice tool for the university's Academic Records Office.

## The Product, as the client asked

The tool allows the user to communicate with the Academic Records Office database, to check if _Syllabus_ records are digitized for any given course, and check if it follows the newly standardized format. Since this format was new, and no other standardized format existed before, the tool is intended to allow an easy upload of a _Syllabus_ document for a course; the program will then parse it as well as it can, to automatically fill in the needed course information. It then allows the user to check if the parsing was correct and edit it to fill in missing or unparsed text.

Technologies used were **Django** as backend framework, **Bootstrap** as frontend framework and **[Tesseract OCR](https://github.com/tesseract-ocr/)** to be able to parse PDFs and scanned documents.

The tool has no name other than "SIGPAE" (Spanish: _Sistema de Gestión de Programas Analíticos de Estudios_) and we signed a confidentiality contract; sadly, I can't show the source code here.

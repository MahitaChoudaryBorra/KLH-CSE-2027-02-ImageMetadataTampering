````markdown
# Image Metadata and Tampering Detection System for Digital Forensic Investigation

## Overview

The Image Metadata and Tampering Detection System is a web-based digital forensic tool designed to analyze the authenticity and reliability of digital images.

The system allows users to upload JPG, JPEG, and PNG images, extracts EXIF metadata, and performs rule-based forensic checks to identify possible signs of image tampering.

The system generates a forensic risk score and classifies images into four categories:

- Safe
- Low Risk
- Suspicious
- Likely Edited

It also generates PDF investigation reports and maintains a searchable history of previous analyses.

## Problem Statement

Digital images shared through social media, messaging applications, and cloud platforms can be modified using image-editing software or metadata manipulation. This makes it difficult to determine their reliability as digital evidence.

Existing forensic tools may require specialized knowledge and often provide raw metadata without an interpretable overall assessment.

This project aims to provide an accessible web-based system that combines EXIF metadata extraction, rule-based forensic checks, risk scoring, and investigation reporting.

## Objectives

- Extract EXIF metadata from uploaded images.
- Analyze camera details, resolution, date and time, GPS information, software, and file properties.
- Detect possible metadata anomalies.
- Identify editing-software signatures.
- Check for inconsistent timestamps.
- Analyze the presence or absence of GPS information.
- Generate a forensic risk score.
- Classify images as Safe, Low Risk, Suspicious, or Likely Edited.
- Generate PDF investigation reports.
- Maintain a searchable history of previous analyses.

## Key Features

### EXIF Metadata Extraction

The system extracts available image metadata including:

- Camera details
- Resolution
- Date and time
- GPS information
- Software information
- File properties

### Rule-Based Forensic Checks

The system checks for possible forensic indicators such as:

- Missing metadata
- Modified metadata
- Editing-software signatures
- Inconsistent timestamps
- Absent GPS information

### Forensic Risk Score

The detected indicators are evaluated using a rule-based scoring mechanism. Based on the resulting score, the image is classified as:

| Classification | Description |
|---|---|
| Safe | No significant suspicious indicators detected |
| Low Risk | Minor suspicious indicators detected |
| Suspicious | Multiple indicators suggest possible manipulation |
| Likely Edited | Strong indicators suggest possible editing |

### PDF Reports

The system generates PDF reports containing the results of the image analysis, metadata information, detected indicators, risk assessment, and classification.

### Analysis History

The system maintains a searchable history of previously analyzed images.

## System Workflow

```text
Upload Image
     |
     v
Validate Image
     |
     v
Extract EXIF Metadata
     |
     v
Perform Forensic Checks
     |
     v
Identify Risk Indicators
     |
     v
Calculate Risk Score
     |
     v
Classify Image
     |
     +------------------+
     |                  |
     v                  v
Generate PDF       Store Analysis
Report             in History
````

## Applications

* Digital forensic investigations
* Journalism and fact-checking
* Insurance claim review
* Forensic science education
* Preliminary image verification
* Digital evidence analysis

## Future Scope

* Machine-learning-based tampering detection
* Error Level Analysis
* Noise-based forensic checks
* Advanced image-content analysis
* Additional metadata consistency checks
* Support for additional image formats
* Advanced forensic reporting

## Team Members

| S. No. | University ID | Name         |
| ------ | ------------- | ------------ |
| 1      | 2320030488    | N. Narasimha |
| 2      | 2320030289    | K. Shivani   |
| 3      | 2320030057    | B. Mahita    |
| 4      | 2320030032    | K. Srikar    |

## Guide

**Dr. N. Chaitanya Kumar**
Department of Computer Science and Engineering
Koneru Lakshmaiah Education Foundation

## Disclaimer

This project is intended for educational purposes and preliminary digital forensic investigation. The generated risk score and classification should be considered decision-support information and should not be treated as conclusive proof of image authenticity or manipulation.


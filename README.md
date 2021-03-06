﻿## Reproducing a Prospective Clinical Study as a Computational Retrospective Study in MIMIC-II
  
This is the repository for the accompanying source code of the AMIA 2015 paper "Reproducing a Prospective Clinical Study as a Computational Retrospective Study in MIMIC-II".
  
The code is composed of two consecutive parts:
* one Java program (headed by HEDICIM.java) that performs the electronic phenotyping from MIMIC-II data and exports a CSV file,
* one R script (hedicim.R) that reads the CSV file and performs the statistical analysis.

As per MIMIC's Data Use Agreement, I am not allowed to provide the CSV file to anyone (e.g. researchers interested only in the statistical analysis part).
  
### Important considerations
* **One source code file is intentionally missing: Keys.java. It contains the username and password for accessing MIMIC-II in the local MySQL server at the U.S. National Library of Medicine. For re-executing the Java code, you will need to obtain your own access to MIMIC-II as per its regulations. If you intend to re-execute the Java code with virtually no modification, you will need MIMIC-II to also be stored in a MySQL server.**
* **Both Java and R programs contain a lot more than what was needed to produce the AMIA 2015 submission. One example, the Java program stores the internal composition of each calculated DIC score (which can be used to produce statistics about the scores). Another example, the Java program produces a file for the EventFlow data visualization program.**
  
Please be welcome to contact Fabrício Kury for help in understanding or reusing the code. Reading and "digesting" code is easily a burdensome task that can become so much easier after a small Skype/Google Hangouts talk with the original programmer (Fabrício) to understand the overall working of the programs.
  
Sincerely,  
Fabrício Kury  
Vojtech Huser  
James Cimino

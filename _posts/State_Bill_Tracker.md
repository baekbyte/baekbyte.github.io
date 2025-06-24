---
title: "State Bill Tracker"
date: 2025-06-23
categories: [AI x Policy Projects]
---

# Introduction

Today, I developed a python program that extracts and tracks US state bills related to artificial intelligence using two different legislative APIs: LegiScan and OpenStates.

## Development Notes

I started by downloading relevant librarys for API calls and dataframes.

```bash
pip install requests pandas openpyxl
```
[**Legiscan**](https://github.com/baekbyte/State-Bill-Tracker/blob/main/legiscan_ai_bill_extractor.py)

For [Legiscan](https://legiscan.com/gaits/documentation/legiscan), I created an account and requested an API key to pull the bills.

Using my API key and the base url, I made two methods to first get the states and the session ids since I need them to search the bills.

<img width="482" alt="Screenshot 2025-06-23 at 9 52 10 PM" src="https://github.com/user-attachments/assets/57a47a89-f300-4977-8018-77ea729e40f4" />

Then, I use both the states and session ids in my search_ai_bills method since Legiscan's getBill documentation requries them as params. Additionally, I added "&query=artificial+intelligence" in the URL in order to only search for AI bills.

<img width="723" alt="Screenshot 2025-06-23 at 9 53 46 PM" src="https://github.com/user-attachments/assets/0c6a834e-05f0-4d9f-9a1b-8a39a1822be6" />

Have extracted the desired bills, I then get those bills' details for the excel sheet.

<img width="464" alt="Screenshot 2025-06-23 at 9 54 32 PM" src="https://github.com/user-attachments/assets/d3908751-14de-45e7-ba1b-46b945042f2a" />

Finally, in my main, I loop through each states and their bills to fetch desired bills and then create a dataframe using pandas to extract them to an excel file

<img width="724" alt="Screenshot 2025-06-23 at 9 55 15 PM" src="https://github.com/user-attachments/assets/49213c7c-9fdd-408e-8efc-f74074b89201" />

I extraced 943 bills using Legiscan's API

[**OpenStates**](https://github.com/baekbyte/State-Bill-Tracker/blob/main/openstates_ai_bill_extractor.py)

For [OpenStates](https://docs.openstates.org/api-v3/), I pretty much used the same framework to extract the bills.

First of all, I created an account to request an API key

Then I use the /jurisdiction root in my get_jurisdiction method to only find all states by adding a "state" classification to my url = f"{BASE_URL}/jurisdictions?classification=state"

<img width="505" alt="Screenshot 2025-06-23 at 9 58 25 PM" src="https://github.com/user-attachments/assets/fe3db28c-6a52-48bc-a7fe-10081e63f545" />

With those jurisdictions, I used the /bills root with certian params to search for AI bills. Then, I loop through every AI bill I have and append more information about them for the excel file.

<img width="795" alt="Screenshot 2025-06-23 at 9 59 55 PM" src="https://github.com/user-attachments/assets/286c5d64-6eab-4365-8df0-7148d45db351" />

Lastly, I call on both methods in my main to extract the AI bills into an excel file using pandas

<img width="652" alt="Screenshot 2025-06-23 at 10 02 44 PM" src="https://github.com/user-attachments/assets/642c27f1-e793-46b1-b8c5-d613af2dcb90" />

*Issue: The abstract query isn't working in my search_ai_bills method*

*OpenStates request limit: Due to this limit, I can only extract a few hundred bills at once*










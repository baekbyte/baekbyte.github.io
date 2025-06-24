---
title: "AI Bill Parser"
date: 2025-06-18
categories: [AI x Policy Projects]
---

# Introduction

Today, I developed a python program that searches through US Congress bill data to find and extract bills related to artificial intelligence.

## Development Notes

I started by installing pandas and openpyxl in order to create data frames and output my data into a excel file

```bash
pip install pandas openpyxl
```

I downloaded JSON files of all congressional bill from 116th-119th Congress from [Legiscan](https://legiscan.com/datasets) and placed them in the "US" folder

<img width="1013" alt="Screenshot 2025-06-23 at 9 40 05 PM" src="https://github.com/user-attachments/assets/5a6c0d9b-b33b-4f52-a7be-d8bb02c3f1e4" />

Then, I developed a simple code to (1) parse through all the JSON files (2) identify bills with the String "Artificial Intelligence" (3) Export them to an excel file

First, I created a method to walk through all the JSON files by using the loop "file in files." Then, I extract the bill title and description to check for "Artificial Intelligence." If the bill contains that string, I then append the ai_bills list with other information.

<img width="815" alt="Screenshot 2025-06-23 at 9 41 31 PM" src="https://github.com/user-attachments/assets/21e0a176-57f5-405e-bd8c-6b193a2c352d" />

With the saved ai_bills, I create a data frame in the save_to_excel method to print all the bills in the excel file using pandas.

<img width="639" alt="Screenshot 2025-06-23 at 9 43 40 PM" src="https://github.com/user-attachments/assets/668b6fe2-aa51-4d1f-a8df-5b90c8b43538" />

In my main, I simply call on both methods and designate the bill directory and the output file

<img width="371" alt="Screenshot 2025-06-23 at 9 44 59 PM" src="https://github.com/user-attachments/assets/d8c75b61-a806-46d4-bd2f-9bdaf286f482" />

As a result I extracted 222 AI bills. Check it out on my [repo](https://github.com/baekbyte/bill-parser)

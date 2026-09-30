1. Form trigger

<img width="1878" height="838" alt="image" src="https://github.com/user-attachments/assets/ee1ddab2-1bd9-4f74-bf70-d80d7ba2dea3" />



2. Fetch PDF File (In your Fetch PDF HTTP Request node, kept the URL field to check or replace AttachLive with AttachHis if needed)

<img width="1907" height="853" alt="image" src="https://github.com/user-attachments/assets/b43496a4-68cb-4a3e-8c11-5acabebf4fd5" />

3. AI Financial Extractor

<img width="1888" height="858" alt="image" src="https://github.com/user-attachments/assets/315857ad-d27e-4c3d-b198-f79fca0c606c" />

[
  {
    "candidates": [
      {
        "content": {
          "parts": [
            {
              "text": "{\n  \"company\": {\n    \"name\": \"Acme Corporation\",\n    \"ticker\": \"ACME\",\n    \"currency\": \"USD\"\n  },\n  \"period\": {\n    \"fiscal_year\": 2023,\n    \"quarter\": \"Q3\",\n    \"start_date\": \"2023-07-01\",\n    \"end_date\": \"2023-09-30\"\n  },\n  \"financial_statement\": {\n    \"revenue\": {\n      \"gross_revenue\": 10500000.00,\n      \"returns_and_discounts\": 500000.00,\n      \"net_revenue\": 10000000.00\n    },\n    \"cost_of_goods_sold\": 4000000.00,\n    \"gross_profit\": 6000000.00,\n    \"operating_expenses\": {\n      \"research_and_development\": 1200000.00,\n      \"sales_and_marketing\": 1800000.00,\n      \"general_and_administrative\": 1000000.00,\n      \"depreciation_and_amortization\": 500000.00,\n      \"total_operating_expenses\": 4500000.00\n    },\n    \"operating_income\": 1500000.00,\n    \"non_operating_items\": {\n      \"interest_expense\": 100000.00,\n      \"tax_expense\": 300000.00,\n      \"total_non_operating_expenses\": 400000.00\n    },\n    \"net_income\": 1100000.00\n  },\n  \"per_share_data\": {\n    \"basic_eps\": 1.10,\n    \"diluted_eps\": 1.05,\n    \"weighted_average_shares_outstanding\": 1000000\n  }\n}",
              "thoughtSignature": "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"
            }
          ],
          "role": "model"
        },
        "finishReason": "STOP",
        "index": 0
      }
    ],
    "usageMetadata": {
      "promptTokenCount": 18,
      "candidatesTokenCount": 512,
      "totalTokenCount": 1478,
      "promptTokensDetails": [
        {
          "modality": "TEXT",
          "tokenCount": 18
        }
      ],
      "thoughtsTokenCount": 948,
      "serviceTier": "standard"
    },
    "modelVersion": "gemini-3.6-flash",
    "responseId": "7G28avepH47RxN8PxpHdiQk"
  }
]

4. Generate HTML Table

<img width="1895" height="836" alt="image" src="https://github.com/user-attachments/assets/14e64d5c-ea3a-443a-acbb-4a0452d619d2" />


<img width="1920" height="876" alt="image" src="https://github.com/user-attachments/assets/ccd23a40-c9a1-4e31-8083-ff87912cdb77" />
<img width="851" height="759" alt="image" src="https://github.com/user-attachments/assets/80c45fc9-2958-4028-a8cb-015294ce3f98" />

5. 

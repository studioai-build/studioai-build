
# Plan Recommendation API

## Request 
```
curl --location 'https://network.studioai.dev/v1/plan-recommendation?insurerId=123' \
--header 'Content-Type: application/json' \
--data '{
    "companyName": "Adam'\''s",
    "address": "Some Address",
    "city": "New York",
    "state": "New York",
    "zipCode": "9999",
    "totalEmployee": "12",
    "effectiveDate": "12 Dec 2023"
}
```

## Response

```json
[
  {
    "name": "Blue PPO Plan",
    "planId": "33380IN0030027",
    "monthlyPrice": "$250",
    "percentMatch": 45,
    "recommendedPercent": 45,
    "recommended": true,
    "description": "Taking into account your group's size, I would recommend our Silver Level Plan. Our analysis shows an 80% closing probability for this plan.",
    "benefits": [
      {
        "title": "Network Type",
        "value": "PPO"
      },
      {
        "title": "Deductible",
        "value": "$3,000"
      },
      {
        "title": "Out-of-pocket Max",
        "value": "$3,000"
      },
      {
        "title": "Primary Care Visits",
        "value": "$25"
      },
      {
        "title": "Speciality Care Visits",
        "value": "$50"
      },
      {
        "title": "Mental Health Visits",
        "value": "$50"
      },
      {
        "title": "Urgent Care",
        "value": "$100"
      },
      {
        "title": "Labs",
        "value": "$25"
      },
      {
        "title": "Generic Drugs",
        "value": "$0"
      }
    ]
  },
  {
    "name": "Bronze Standardized",
    "planId": "33380IN0030090",
    "monthlyPrice": "$269",
    "percentMatch": 55,
    "recommendedPercent": 55,
    "recommended": true,
    "description": "Based on your group's characteristics and preferences, we predict a 78% chance of success if we proceed with the Gold Plan.",
    "benefits": [
      {
        "title": "Network Type",
        "value": "PPO"
      },
      {
        "title": "Deductible",
        "value": "$3,200"
      },
      {
        "title": "Out-of-pocket Max",
        "value": "$3,000"
      },
      {
        "title": "Primary Care Visits",
        "value": "$25"
      },
      {
        "title": "Speciality Care Visits",
        "value": "$40"
      },
      {
        "title": "Mental Health Visits",
        "value": "$50"
      },
      {
        "title": "Urgent Care",
        "value": "$100"
      },
      {
        "title": "Labs",
        "value": "$50"
      },
      {
        "title": "Generic Drugs",
        "value": "$0"
      }
    ]
  },
  {
    "name": "Silver HSA 3000 - 1 Plus",
    "planId": "33380IN0050013",
    "monthlyPrice": "$296",
    "percentMatch": 75,
    "recommendedPercent": 75,
    "recommended": true,
    "description": "If your group's main concern is affordability, our Economy Plan is a viable option. With a 70% probability of closing, according to our AI predictions, this could be an excellent choice for your team.",
    "benefits": [
      {
        "title": "Network Type",
        "value": "PPO"
      },
      {
        "title": "Deductible",
        "value": "$2,800"
      },
      {
        "title": "Out-of-pocket Max",
        "value": "$2,500"
      },
      {
        "title": "Primary Care Visits",
        "value": "$60"
      },
      {
        "title": "Speciality Care Visits",
        "value": "$60"
      },
      {
        "title": "Mental Health Visits",
        "value": "$50"
      },
      {
        "title": "Urgent Care",
        "value": "$50"
      },
      {
        "title": "Labs",
        "value": "$30"
      },
      {
        "title": "Generic Drugs",
        "value": "$0"
      }
    ]
  },
  {
    "name": "Silver H.S.A. 2700 Basic Plus",
    "planId": "33380IN0050010",
    "monthlyPrice": "$329",
    "percentMatch": 85,
    "recommendedPercent": 85,
    "recommended": false,
    "description": "Given your company size, this plan provides lower premiums, improved preventive care, tailored coverage based on population health data, and broad network access.",
    "benefits": [
      {
        "title": "Network Type",
        "value": "PPO"
      },
      {
        "title": "Deductible",
        "value": "$4,000"
      },
      {
        "title": "Out-of-pocket Max",
        "value": "$5,000"
      },
      {
        "title": "Primary Care Visits",
        "value": "$60"
      },
      {
        "title": "Speciality Care Visits",
        "value": "$50"
      },
      {
        "title": "Mental Health Visits",
        "value": "$50"
      },
      {
        "title": "Urgent Care",
        "value": "$80"
      },
      {
        "title": "Labs",
        "value": "$20"
      },
      {
        "title": "Generic Drugs",
        "value": "$0"
      }
    ]
  }
]
```


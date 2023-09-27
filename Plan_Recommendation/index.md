
# Plan Recommendation API


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

**Response**

```
[
  {
    "name": "Blue PPO Plan A",
    "planId": "33380IN0030022",
    "monthlyPrice": "$250",
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
    "name": "Blue PPO Plan B",
    "planId": "33380IN0050001",
    "monthlyPrice": "$269",
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
    "name": "Blue PPO Plan C",
    "planId": "33380IN0030016",
    "monthlyPrice": "$296",
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
    "name": "Blue PPO Plan D",
    "planId": "33380IN0030027",
    "monthlyPrice": "$329",
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


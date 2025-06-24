# Deloitte Australia – Data Analytics Virtual Internship (via Forage)

This repository contains my completed work for the **Deloitte Australia – Data Analytics Job Simulation** hosted on [Forage](https://www.theforage.com/).

Over this virtual internship, I solved real-world problems faced by Deloitte clients across two major tasks: telemetry analysis and forensic pay equality review.

---

## 💼 Internship Tasks

### 🔹 Task 1: Telemetry Data Analysis (Daikibo Case)
- **Client**: Daikibo Industries (Global manufacturing firm)
- **Objective**: Analyze telemetry data from 4 international factories to:
  1. Identify which factory experienced the most machine breakdowns.
  2. Discover which machine types failed most often at that factory.
- **Tools Used**: Tableau, JSON, Data Visualization
- **Output**:
  - A bar chart comparing downtime by factory.
  - A filtered dashboard showing downtime by machine type.

📁 Files:
- [daikibo-telemetry-sample.json](https://github.com/user-attachments/files/20884621/daikibo-telemetry-sample.json)[
  {
    "deviceID": "19ff3161-2b3a-40a3-8604-bdc6532d0dab",
    "deviceType": "CNC",
    "timestamp": 1619816400000,
    "location": {
      "country": "japan",
      "city": "tokyo",
      "area": "keiyō-industrial-zone",
      "factory": "daikibo-factory-meiyo",
      "section": "section-1"
    },
    "data": {
      "status": "healthy",
      "temperature": 27
    }
  },
  {
    "deviceID": "19ff3161-2b3a-40a3-8604-bdc6532d0dab",
    "deviceType": "CNC",
    "timestamp": 1619817000000,
    "location": {
      "country": "japan",
      "city": "tokyo",
      "area": "keiyō-industrial-zone",
      "factory": "daikibo-factory-meiyo",
      "section": "section-1"
    },
    "data": {
      "status": "healthy",
      "temperature": 27
    }
  },
  {
    "deviceID": "19ff3161-2b3a-40a3-8604-bdc6532d0dab",
    "deviceType": "CNC",
    "timestamp": 1619817600000,
    "location": {
      "country": "japan",
      "city": "tokyo",
      "area": "keiyō-industrial-zone",
      "factory": "daikibo-factory-meiyo",
      "section": "section-1"
    },
    "data": {
      "status": "healthy",
      "temperature": 26
    }
  },
  {
    "deviceID": "19ff3161-2b3a-40a3-8604-bdc6532d0dab",
    "deviceType": "CNC",
    "timestamp": 1619818200000,
    "location": {
      "country": "japan",
      "city": "tokyo",
      "area": "keiyō-industrial-zone",
      "factory": "daikibo-factory-meiyo",
      "section": "section-1"
    },
    "data": {
      "status": "healthy",
      "temperature": 24
    }
  },
  {
    "deviceID": "19ff3161-2b3a-40a3-8604-bdc6532d0dab",
    "deviceType": "CNC",
    "timestamp": 1619818800000,
    "location": {
      "country": "japan",
      "city": "tokyo",
      "area": "keiyō-industrial-zone",
      "factory": "daikibo-factory-meiyo",
      "section": "section-1"
    },
    "data": {
      "status": "healthy",
      "temperature": 27
    }
  },
  {
    "deviceID": "19ff3161-2b3a-40a3-8604-bdc6532d0dab",
    "deviceType": "CNC",
    "timestamp": 1619819400000,
    "location": {
      "country": "japan",
      "city": "tokyo",
      "area": "keiyō-industrial-zone",
      "factory": "daikibo-factory-meiyo",
      "section": "section-1"
    },
    "data": {
      "status": "healthy",
      "temperature": 26
    }
  },
  {
    "deviceID": "19ff3161-2b3a-40a3-8604-bdc6532d0dab",
    "deviceType": "CNC",
    "timestamp": 1619820000000,
    "location": {
      "country": "japan",
      "city": "tokyo",
      "area": "keiyō-industrial-zone",
      "factory": "daikibo-factory-meiyo",
      "section": "section-1"
    },
    "data": {
      "status": "healthy",
      "temperature": 25
    }
  },
  {
    "deviceID": "19ff3161-2b3a-40a3-8604-bdc6532d0dab",
    "deviceType": "CNC",
    "timestamp": 1619820600000,
    "location": {
      "country": "japan",
      "city": "tokyo",
      "area": "keiyō-industrial-zone",
      "factory": "daikibo-factory-meiyo",
      "section": "section-1"
    },
    "data": {
      "status": "healthy",
      "temperature": 23
    }
  },
  {
    "deviceID": "19ff3161-2b3a-40a3-8604-bdc6532d0dab",
    "deviceType": "CNC",
    "timestamp": 1619821200000,
    "location": {
      "country": "japan",
      "city": "tokyo",
      "area": "keiyō-industrial-zone",
      "factory": "daikibo-factory-meiyo",
      "section": "section-1"
    },
    "data": {
      "status": "healthy",
      "temperature": 26
    }
  },
  {
    "deviceID": "19ff3161-2b3a-40a3-8604-bdc6532d0dab",
    "deviceType": "CNC",
    "timestamp": 1619821800000,
    "location": {
      "country": "japan",
      "city": "tokyo",
      "area": "keiyō-industrial-zone",
      "factory": "daikibo-factory-meiyo",
      "section": "section-1"
    },
    "data": {
      "status": "healthy",
      "temperature": 26
    }
  },
  {
    "deviceID": "19ff3161-2b3a-40a3-8604-bdc6532d0dab",
    "deviceType": "CNC",
    "timestamp": 1619822400000,
    "location": {
      "country": "japan",
      "city": "tokyo",
      "area": "keiyō-industrial-zone",
      "factory": "daikibo-factory-meiyo",
      "section": "section-1"
    },
    "data": {
      "status": "healthy",
      "temperature": 25
    }
  },
  {
    "deviceID": "19ff3161-2b3a-40a3-8604-bdc6532d0dab",
    "deviceType": "CNC",
    "timestamp": 1619823000000,
    "location": {
      "country": "japan",
      "city": "tokyo",
      "area": "keiyō-industrial-zone",
      "factory": "daikibo-factory-meiyo",
      "section": "section-1"
    },
    "data": {
      "status": "healthy",
      "temperature": 24
    }
  },
  {
    "deviceID": "19ff3161-2b3a-40a3-8604-bdc6532d0dab",
    "deviceType": "CNC",
    "timestamp": 1619823600000,
    "location": {
      "country": "japan",
      "city": "tokyo",
      "area": "keiyō-industrial-zone",
      "factory": "daikibo-factory-meiyo",
      "section": "section-1"
    },
    "data": {
      "status": "healthy",
      "temperature": 27
    }
  },
  {
    "deviceID": "19ff3161-2b3a-40a3-8604-bdc6532d0dab",
    "deviceType": "CNC",
    "timestamp": 1619824200000,
    "location": {
      "country": "japan",
      "city": "tokyo",
      "area": "keiyō-industrial-zone",
      "factory": "daikibo-factory-meiyo",
      "section": "section-1"
    },
    "data": {
      "status": "healthy",
      "temperature": 27
    }
  },
  {
    "deviceID": "19ff3161-2b3a-40a3-8604-bdc6532d0dab",
    "deviceType": "CNC",
    "timestamp": 1619824800000,
    "location": {
      "country": "japan",
      "city": "tokyo",
      "area": "keiyō-industrial-zone",
      "factory": "daikibo-factory-meiyo",
      "section": "section-1"
    },
    "data": {
      "status": "healthy",
      "temperature": 26
    }
  },
  {
    "deviceID": "19ff3161-2b3a-40a3-8604-bdc6532d0dab",
    "deviceType": "CNC",
    "timestamp": 1619825400000,
    "location": {
      "country": "japan",
      "city": "tokyo",
      "area": "keiyō-industrial-zone",
      "factory": "daikibo-factory-meiyo",
      "section": "section-1"
    },
    "data": {
      "status": "healthy",
      "temperature": 23
    }
  },
  {
    "deviceID": "19ff3161-2b3a-40a3-8604-bdc6532d0dab",
    "deviceType": "CNC",
    "timestamp": 1619826000000,
    "location": {
      "country": "japan",
      "city": "tokyo",
      "area": "keiyō-industrial-zone",
      "factory": "daikibo-factory-meiyo",
      "section": "section-1"
    },
    "data": {
      "status": "healthy",
      "temperature": 24
    }
  },
  {
    "deviceID": "19ff3161-2b3a-40a3-8604-bdc6532d0dab",
    "deviceType": "CNC",
    "timestamp": 1619826600000,
    "location": {
      "country": "japan",
      "city": "tokyo",
      "area": "keiyō-industrial-zone",
      "factory": "daikibo-factory-meiyo",
      "section": "section-1"
    },
    "data": {
      "status": "healthy",
      "temperature": 27
    }
  },
  {
    "deviceID": "19ff3161-2b3a-40a3-8604-bdc6532d0dab",
    "deviceType": "CNC",
    "timestamp": 1619827200000,
    "location": {
      "country": "japan",
      "city": "tokyo",
      "area": "keiyō-industrial-zone",
      "factory": "daikibo-factory-meiyo",
      "section": "section-1"
    },
    "data": {
      "status": "healthy",
      "temperature": 25
    }
  },
  {
    "deviceID": "19ff3161-2b3a-40a3-8604-bdc6532d0dab",
    "deviceType": "CNC",
    "timestamp": 1619827800000,
    "location": {
      "country": "japan",
      "city": "tokyo",
      "area": "keiyō-industrial-zone",
      "factory": "daikibo-factory-meiyo",
      "section": "section-1"
    },
    "data": {
      "status": "healthy",
      "temperature": 23
    }
  },
  {
    "deviceID": "19ff3161-2b3a-40a3-8604-bdc6532d0dab",
    "deviceType": "CNC",
    "timestamp": 1619828400000,
    "location": {
      "country": "japan",
      "city": "tokyo",
      "area": "keiyō-industrial-zone",
      "factory": "daikibo-factory-meiyo",
      "section": "section-1"
    },
    "data": {
      "status": "healthy",
      "temperature": 26
    }
  },
  {
    "deviceID": "19ff3161-2b3a-40a3-8604-bdc6532d0dab",
    "deviceType": "CNC",
    "timestamp": 1619829000000,
    "location": {
      "country": "japan",
      "city": "tokyo",
      "area": "keiyō-industrial-zone",
      "factory": "daikibo-factory-meiyo",
      "section": "section-1"
    },
    "data": {
      "status": "healthy",
      "temperature": 26
    }
  },
  {
    "deviceID": "19ff3161-2b3a-40a3-8604-bdc6532d0dab",
    "deviceType": "CNC",
    "timestamp": 1619829600000,
    "location": {
      "country": "japan",
      "city": "tokyo",
      "area": "keiyō-industrial-zone",
      "factory": "daikibo-factory-meiyo",
      "section": "section-1"
    },
    "data": {
      "status": "healthy",
      "temperature": 23
    }
  },
  {
    "deviceID": "19ff3161-2b3a-40a3-8604-bdc6532d0dab",
    "deviceType": "CNC",
    "timestamp": 1619830200000,
    "location": {
      "country": "japan",
      "city": "tokyo",
      "area": "keiyō-industrial-zone",
      "factory": "daikibo-factory-meiyo",
      "section": "section-1"
    },
    "data": {
      "status": "healthy",
      "temperature": 24
    }
  },
  {
    "deviceID": "19ff3161-2b3a-40a3-8604-bdc6532d0dab",
    "deviceType": "CNC",
    "timestamp": 1619830800000,
    "location": {
      "country": "japan",
      "city": "tokyo",
      "area": "keiyō-industrial-zone",
      "factory": "daikibo-factory-meiyo",
      "section": "section-1"
    },
    "data": {
      "status": "healthy",
      "temperature": 24
    }
  },
  {
    "deviceID": "19ff3161-2b3a-40a3-8604-bdc6532d0dab",
    "deviceType": "CNC",
    "timestamp": 1619831400000,
    "location": {
      "country": "japan",
      "city": "tokyo",
      "area": "keiyō-industrial-zone",
      "factory": "daikibo-factory-meiyo",
      "section": "section-1"
    },
    "data": {
      "status": "healthy",
      "temperature": 24
    }
  },
  {
    "deviceID": "19ff3161-2b3a-40a3-8604-bdc6532d0dab",
    "deviceType": "CNC",
    "timestamp": 1619832000000,
    "location": {
      "country": "japan",
      "city": "tokyo",
      "area": "keiyō-industrial-zone",
      "factory": "daikibo-factory-meiyo",
      "section": "section-1"
    },
    "data": {
      "status": "healthy",
      "temperature": 26
    }
  },
  {
    "deviceID": "19ff3161-2b3a-40a3-8604-bdc6532d0dab",
    "deviceType": "CNC",
    "timestamp": 1619832600000,
    "location": {
      "country": "japan",
      "city": "tokyo",
      "area": "keiyō-industrial-zone",
      "factory": "daikibo-factory-meiyo",
      "section": "section-1"
    },
    "data": {
      "status": "healthy",
      "temperature": 27
    }
  },
  {
    "deviceID": "19ff3161-2b3a-40a3-8604-bdc6532d0dab",
    "deviceType": "CNC",
    "timestamp": 1619833200000,
    "location": {
      "country": "japan",
      "city": "tokyo",
      "area": "keiyō-industrial-zone",
      "factory": "daikibo-factory-meiyo",
      "section": "section-1"
    },
    "data": {
      "status": "healthy",
      "temperature": 24
    }
  },
  {
    "deviceID": "19ff3161-2b3a-40a3-8604-bdc6532d0dab",
    "deviceType": "CNC",
    "timestamp": 1619833800000,
    "location": {
      "country": "japan",
      "city": "tokyo",
      "area": "keiyō-industrial-zone",
      "factory": "daikibo-factory-meiyo",
      "section": "section-1"
    },
    "data": {
      "status": "healthy",
      "temperature": 27
    }
  },
  {
    "deviceID": "19ff3161-2b3a-40a3-8604-bdc6532d0dab",
    "deviceType": "CNC",
    "timestamp": 1619834400000,
    "location": {
      "country": "japan",
      "city": "tokyo",
      "area": "keiyō-industrial-zone",
      "factory": "daikibo-factory-meiyo",
      "section": "section-1"
    },
    "data": {
      "status": "healthy",
      "temperature": 23
    }
  },
  {
    "deviceID": "19ff3161-2b3a-40a3-8604-bdc6532d0dab",
    "deviceType": "CNC",
    "timestamp": 1619835000000,
    "location": {
      "country": "japan",
      "city": "tokyo",
      "area": "keiyō-industrial-zone",
      "factory": "daikibo-factory-meiyo",
      "section": "section-1"
    },
    "data": {
      "status": "healthy",
      "temperature": 27
    }
  },
  {
    "deviceID": "19ff3161-2b3a-40a3-8604-bdc6532d0dab",
    "deviceType": "CNC",
    "timestamp": 1619835600000,
    "location": {
      "country": "japan",
      "city": "tokyo",
      "area": "keiyō-industrial-zone",
      "factory": "daikibo-factory-meiyo",
      "section": "section-1"
    },
    "data": {
      "status": "healthy",
      "temperature": 26
    }
  },
  {
    "deviceID": "19ff3161-2b3a-40a3-8604-bdc6532d0dab",
    "deviceType": "CNC",
    "timestamp": 1619836200000,
    "location": {
      "country": "japan",
      "city": "tokyo",
      "area": "keiyō-industrial-zone",
      "factory": "daikibo-factory-meiyo",
      "section": "section-1"
    },
    "data": {
      "status": "healthy",
      "temperature": 23
    }
  },
  {
    "deviceID": "19ff3161-2b3a-40a3-8604-bdc6532d0dab",
    "deviceType": "CNC",
    "timestamp": 1619836800000,
    "location": {
      "country": "japan",
      "city": "tokyo",
      "area": "keiyō-industrial-zone",
      "factory": "daikibo-factory-meiyo",
      "section": "section-1"
    },
    "data": {
      "status": "healthy",
      "temperature": 26
    }
  },
  {
    "deviceID": "19ff3161-2b3a-40a3-8604-bdc6532d0dab",
    "deviceType": "CNC",
    "timestamp": 1619837400000,
    "location": {
      "country": "japan",
      "city": "tokyo",
      "area": "keiyō-industrial-zone",
      "factory": "daikibo-factory-meiyo",
      "section": "section-1"
    },
    "data": {
      "status": "healthy",
      "temperature": 27
    }
  }
]
> ⚠️ **Note:** The original JSON file was too large for full preview in GitHub. This is a sample version of the original JSON telemetry file.

Only the first few hundred lines are included for reference due to GitHub size limitations.

The full file can be provided upon request.

- ![Task 1 Ouput](https://github.com/user-attachments/assets/24f3e915-d1bc-4a1a-8f9f-5fbef5f695f6)


---

### 🔹 Task 2: Forensic Technology – Pay Equality Classification
- **Objective**: Use employee compensation data to classify fairness in pay.
- **Context**: Investigate internal complaints of gender-based salary inequality.
- **Work Done**:
  - Created a new column (`Equality Class`) in Excel.
  - Classified roles into `Fair`, `Unfair`, or `Highly Discriminative` based on equality score thresholds.
- **Tools Used**: Microsoft Excel (functions, logical conditions)

📁 File:
- [Task 2 Equality Table.xlsx](https://github.com/user-attachments/files/20884407/Task.2.Equality.Table.xlsx)


---

## 🧠 Skills Gained

- Data Analysis & Interpretation  
- Business Intelligence with Tableau  
- Risk Assessment & Classification  
- Excel Logical Functions  
- Data Storytelling & Reporting  
- Consulting-style Problem Solving  

---

## 📄 Certificate

![Certificate](https://github.com/user-attachments/assets/f3608148-ceb0-42af-a4ee-cb05225d0553)


- **Issued By**: Deloitte Australia (via Forage)
- **Completion Date**: June 3rd, 2025

---

## 🧭 About This Internship

This virtual internship offered an immersive experience in Deloitte’s consulting work. It helped me develop hands-on skills through client-simulated challenges and build confidence in applying analytics to solve real-world problems.

---

## 📬 Contact Me

Connect with me on [LinkedIn](www.linkedin.com/in/kashish-yadav-4a9125251)  
Feel free to explore the repo and share feedback!

---

## 🏷️ Tags

`#Deloitte` `#DataAnalytics` `#VirtualInternship` `#ForensicTechnology` `#Excel` `#Tableau` `#GitHubProject` `#KashishYadav`

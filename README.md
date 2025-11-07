📱 App Review Sentiment Tracker (n8n Workflow)

🚀 Overview
This n8n workflow automates the process of fetching app reviews from the App Store, analyzing their sentiment, and storing the results in Google Sheets. It also generates a weekly sentiment summary for Product Managers.

⚙️ Workflow Steps
1. Schedule Trigger → Runs daily at 9 AM  
2. HTTP Request → Fetches App Store reviews (JSON feed)  
3. Function Node → Parses and cleans review data  
4. Function Node → Applies sentiment analysis logic  
5. Google Sheets Node → Stores reviews and sentiment results  
6. (Optional) Weekly workflow → Generates summary email

🧠 Tools Used
- n8n – workflow automation platform  
- Apple RSS API – source of app reviews  
- Google Sheets – data storage  
- JavaScript (Function Nodes) – for parsing and sentiment logic  
- Gmail/Slack – for weekly report delivery


🤖 How AI is Used
The workflow uses simple text classification logic to label each review as positive, neutral, or negative.  
It can be upgraded to use OpenAI or Google Cloud Natural Language for more advanced sentiment detection.


 📸 Visual Workflow
https://app.eraser.io/workspace/xOKRY11AvbDVCTzabbMH

📊 Output Example
| Review | Rating | Sentiment |
|--------|---------|-----------|
| “Love the new UI!” | ⭐⭐⭐⭐⭐ | Positive |
| “App keeps crashing” | ⭐ | Negative |

⚠️ Limitations
- API only fetches latest 50 reviews per region
- Sarcasm and non-English text may misclassify
- Google Sheets performance declines after 10k+ rows

🧩 How to Use
1. Download `AppReviewSentimentTracker.json`
2. Import into your n8n instance (File → Import from File)
3. Add your Google credentials
4. Execute the workflow


🧷 Links
- Visual design: [Whimsical Workflow Diagram](https://app.eraser.io/workspace/xOKRY11AvbDVCTzabbMH)
- Video walkthrough: (Add your video or LinkedIn post link here)

👨‍💻 Author
Created by [Your Name](https://www.linkedin.com/in/your-profile/) 
#n8n #Automation #AI #ProductManagement #WorkflowAutomation

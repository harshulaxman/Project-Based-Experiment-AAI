<H3>ENTER YOUR NAME: Harsshitha lakshmanan</H3>
<H3>ENTER YOUR REGISTER NO.: 212223230075</H3>
<H3>DATE:16-11-2025</H3>
<H1 Align="center">Project Based Experiment<H1>
  
## Objective
The objective of this project is to perform sentiment analysis on my extracted Facebook data and to count the number of occurrences of my name in the text using Python. This helps understand text polarity and analyze personal mentions in social media data.
## Program:
  
``` Python
import re
from textblob import TextBlob

with open("facebook_data.txt", "r", encoding="utf8") as file:
    fb_text = file.read()

blob = TextBlob(fb_text)

your_name = "Harsshitha"  
pattern = re.compile(rf"\b{your_name}\b", re.IGNORECASE)
name_count = len(pattern.findall(fb_text))

print("Sentiment Score:", sentiment_score)
print(f"Occurrences of '{your_name}':", name_count)
```

## Output:
<img width="447" height="66" alt="image" src="https://github.com/user-attachments/assets/e63e338a-4cf0-45b4-b4e4-e22b4df24160" />

## Inference:
From this project, I learned how to extract and process text data from social media sources, specifically Facebook. I understood how sentiment analysis works using TextBlob and how polarity scores indicate whether text is positive, negative, or neutral. I also learned how to write simple text-processing scripts using Python, including counting specific word occurrences with regular expressions. Overall, this project improved my understanding of natural language processing and analyzing personal social media data.

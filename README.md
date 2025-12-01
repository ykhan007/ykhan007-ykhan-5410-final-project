# Markov News Headline Generator

This project generates short, news-style headlines using a Markov Chain model.  
I created this project for my Algorithms course (BSSD 3410/5410) based on the Markov Text Generator topic we covered in Week 13.

The idea is simple: the program reads several old newspaper-style text files, learns how words usually follow each other, and then uses that pattern to generate new headlines that *sound* like they came from those newspapers.

---

## How the Project Works

### 1. Data Sources
I used three public-domain–style U.S. news text files (not used in class):

- **American Tribune Report – 1915**  
- **Washington Herald Dispatch – 1920**  
- **National Gazette Bulletin – 1912**

All three files are combined into a single word list (corpus).  
This gives the Markov model enough variety to generate natural-looking headlines.

### 2. Markov Chain Logic
The program works by looking at sequences of 3 words (window size = 3).  
For every sequence, it records what word usually comes next.

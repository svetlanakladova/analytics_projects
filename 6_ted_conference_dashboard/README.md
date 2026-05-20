# TED Conference Analytics Dashboard

### [Presentation](https://datalens.yandex/p8nc6j6j525yb)

### Project Overview

This project focuses on building an analytical dashboard for TED conference data.

A company purchased a license to organize TED-style conferences and wanted to better understand how successful TED events are structured. The goal was to analyze past TED conferences and create a dashboard that helps organizers make data-driven decisions about speakers, topics, and event planning.

The dashboard was built to support business decisions related to:
- conference themes
- speaker selection
- audience engagement
- event structure and timing

---

## Business Questions

- Which TED topics are the most popular?
- How do viewers react to different topics?
- What is the average number of speakers per conference?
- What is the average talk duration?
- Which speakers receive the most audience engagement?
- Which talks are the funniest or most popular?
- Which speaker occupations attract the most applause?

---

### Dashboard Features

**High-level metrics:**
- Number of conferences
- Number of talks
- Number of unique speakers
- Number of tags/topics

**Detailed conference-level analysis:**
- Average talk duration
- Maximum talk views
- Total applause count
- Number of speakers per conference

**The dashboard includes:**
- Top 10 funniest talks
- Top 20 most popular tags
- Detailed talk-level information

**Analysis of speaker engagement:**
- Most applauded speakers
- Speaker occupations
- Audience reaction metrics

**The dashboard includes filters for:**
- Country
- Conference name
- Talk tag
- Recording date

---

### Dataset Description

The project uses three datasets:

<img width="2880" height="1324" alt="Image (1)" src="https://github.com/user-attachments/assets/1cd2f60e-c9d8-45be-8b0b-68996e1648f3" />

`events` — conference information:
- `conf_id` — conference ID
- `event_name` — conference name
- `country` — conference country

`speakers` — speaker information:
- `author_id` — speaker ID
- `speaker_name` — speaker name
- `speaker_occupation` — speaker occupation
- `speaker_description` — speaker description

`talks` — talk-level information:
- `talk_id` — talk ID
- `url` — public TED talk URL
- `title` — talk title
- `description` — talk description
- `film_date` — recording date
- `duration` — talk duration
- `views_count` — number of views
- `main_tag` — main talk topic
- `speaker_id` — speaker identifier
- `laughter_count` — number of laughter reactions
- `applause_count` — number of applause reactions
- `language_sp` — talk language
- `event_id` — conference identifier

---

### Project Structure

1. Data preparation and validation  
2. SQL data model creation  
3. Table joins and metric calculation  
4. Dashboard development in DataLens  
5. Interactive filters and drill-down setup  
6. Business insights and recommendations  

---

### Key Insights

- The dataset includes 327 TED conferences, 3377 talks, and 2943 unique speakers across 80 different topics
- The most popular TED topics are science, technology, and culture
- TED2006 (United States) hosted the most viewed talk in the dataset with more than 72 million views
- Audience engagement is strongly connected to entertaining and emotional presentations
- “All things are Moleeds” is one of the funniest talks based on audience laughter reactions
- Most conferences feature a wide variety of speakers and topics, showing the diversity of TED events

---

### Tools & Technologies

`SQL` `Yandex DataLens` 

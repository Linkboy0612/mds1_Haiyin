# 1. Project Overview

This project collects social media data from **YouTube** for the purpose of conducting a sentiment analysis as part of Assignment 1.

The dataset contains metadata and textual content from YouTube videos related to the topic **"Artificial Intelligence"**.

All data was collected using the **official YouTube Data API v3**, following ethical and platform‑compliant data collection practices.

# 2. API Used

**YouTube Data API v3**

* Official Google API
* Used to retrieve video metadata, statistics, and textual content
* Endpoints used:
  * `search.list` (to search for videos)
  * `videos.list` (to retrieve detailed metadata and engagement metrics)

# 3. Authentication Method

The script uses an **API Key** stored securely in a local `.env` file. 

The key is **not hard‑coded** in the script to avoid exposing credentials.

Environment variable used: `YOUTUBE_API_KEY`


# 4. Keywords

The following keyword was used to retrieve relevant YouTube videos:

* **Artificial Intelligence**

This keyword was chosen because it represents a widely discussed public topic with rich user‑generated content suitable for sentiment analysis.

# 5. Date Range

The YouTube API was queried using:

* **order = "date"**, which retrieves videos sorted by upload time
* No explicit `publishedAfter` filter was applied
* Therefore, the dataset includes **recent videos returned by the API at the time of collection**

Collection date:

* **29 May 2026 (local time)**

# 6. Number of Records Collected

A total of: 

**144 video records**

were successfully collected, meeting the assignment requirement of **at least 100 records**.

# 7. Dataset Fields

The final dataset includes the following fields, all required or recommended by the assignment brief:

| Field Name | Description |
| --- | --- |
| `video_id` | Unique ID of the YouTube video |
| `title` | Video title (text content for analysis) |
| `description` | Video description (text content for analysis) |
| `published_at` | Upload timestamp |
| `channel_title` | Name of the channel (author) |
| `view_count` | Number of views |
| `like_count` | Number of likes |
| `comment_count` | Number of comments |
| `url` | Direct link to the video |
| `platform` | Platform name ("YouTube") |
| `keyword` | Search keyword used ("Artificial Intelligence") |
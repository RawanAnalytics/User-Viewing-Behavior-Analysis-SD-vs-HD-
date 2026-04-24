## Project Background :
Telecom Company STC was established in 1998 and is a leading Saudi telecommunications company offering a diverse range of communications, internet and data solutions.
STCtv is its entertainment platform, offering a variety of movies and series.

This project was completed as part of a virtual data analytics experience program with STC, simulating real-world data analysis tasks.

The objective of this task is to analyze user viewing behavior and identify:
- Users who prefer to watch in SD quality
- Users who prefer to watch in HD quality

This analysis aims to support improving STCtv service performance and user experience by understanding content consumption patterns.

## Data Structure :
This project processes a large-scale dataset exceeding one million records.

To facilitate quick review, a sample dataset is provided:
User_Viewing_Behavior_Sample_data.zip
The code is designed to efficiently handle the full dataset.

#### Input Columns :
| Column Name        | Description |
|-------------------|------------|
| Column 1          | Index|
| date_             | The date when the user watched the content |
| user_id_maped     | Unique anonymized user ID |
| program_name      | Name of the content |
| duration_seconds  | Viewing duration in seconds |
| program_class     | Content type (Movie or Series/Episodes) |
| season            | Season number (for series) |
| episode           | Episode number (for series) |
| program_desc      | Content description |
| program_genre     | Content genre |
| series_title      | 1 = title includes extra details (season,episode), 0 = title is clean without additional information|
| hd                | 1 = HD, 0 = SD |
| original_name     | Original content name |


## methodology :
The analysis was performed using a combination of Python and Excel pivot tables.
### Python Data Processing:
Before performing the analysis in Excel, the Python  was used to clean, transform, and aggregate the raw data:
- Extracting data from a compressed file.
- cleaned and structured The dataset.
- Episode and season information combined to uniquely identify series content.
- Grouped data using aggregation functions to calculate:
  - Number of Users who Watched	.
  - Number of watches.
  - Total watch time in houres.
- Sorting and preparing data for further analysis
This step ensured the dataset was optimized and ready for efficient analysis.


### Excel Pivot Table Analysis :
The processed data was then exported to Excel, where Pivot Tables were used to segment and analyze the data into:
- SD vs HD Users.
- Movies vs Series/Episodes.
- Program Genre.
#### Key Metrics Analyzed:
- Number of Users	.
- Number of Views.
- Total watch time in houres.
#### Each metric was further analyzed using :
- Total values.
- Average values.

#### Key Visuals :

<img width="568" height="685" alt="image" src="https://github.com/user-attachments/assets/c954b59f-955e-4457-912c-9bc032858cd2" />


Full detailed pivot tables are available in the Excel results file included in the repository


## Executive Summary :
The analysis reveals clear behavioral differences between HD and SD users.
- HD users tend to prefer watching movies
- SD users tend to prefer watching series and episodes
Across both quality types:
The most popular genres are action and animation.
The insight highlights strong consistency regardless of streaming quality.

### HD Users :
Prefer movies over series.
#### Top genres :
- Action
- Animation
### SD Users :
Prefer series/Episodes over movies.
#### Top genres :
- Action
- Animation
#### Highest watch time observed in :
Drama

### Overall Insights :
#### Most popular genres :
- Action
- Animation

#### Action genres :
- Total Users: 91,450
- Total Views: 172,680
- Total Watch Time (hours): 76,394 / 52,472

#### Animation genres :
- Total Users: 147,653
- Total Views: 401,932
- Total Watch Time (hours): 90,079 / 25


## Recommendations :
- Focus on action and animation content, whether it's movies or series, since both types of users prefer them.
- Customize recommendations based on user quality preferences (HD vs SD).
- Improving platform performance for types of content that require long viewing times, such as drama.
- Enhancing the HD movie streaming experience for HD users.
- Improved series recommendations for SD users.



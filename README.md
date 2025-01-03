# YouTube Channel Analysis

This project performs an analysis of YouTube channel data and video details using the YouTube Data API. The goal is to fetch data about various YouTube channels, perform exploratory data analysis (EDA), and visualize key metrics such as views, subscribers, video counts, and channel age. The project also dives deep into the most subscribed YouTuber, Zakir Khan, and performs EDA on his video data.

## Table of Contents
- [Project Overview](#project-overview)
- [Installation](#installation)
- [Usage](#usage)
- [Data Analysis](#data-analysis)
- [Visualization](#visualization)
- [Data Export](#data-export)
- [Contributing](#contributing)
- [Google Colab Link for Project](#ColabLink)

## Project Overview

This project involves analyzing the YouTube channels of several stand-up comedians, including the most popular comedian on the platform, Zakir Khan. The main steps include:

1. **Fetching Channel Data**: Using the YouTube API to fetch data such as views, subscribers, total videos, and channel age for various comedians.
2. **Data Formatting**: Cleaning and organizing the fetched data for easier analysis.
3. **Exploratory Data Analysis (EDA)**: Using pandas to explore correlations between different features of the channel data.
4. **Visualization**: Creating various visualizations using Matplotlib and Seaborn to present insights about the YouTube channels and videos.
5. **Zakir Khan's Video Analysis**: Fetching detailed information about all videos uploaded by Zakir Khan, performing EDA, and visualizing the data.

Additionally, all the collected data is exported into CSV files for easy reference.

## Installation

To run this project locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/youtube-channel-analysis.git
   cd youtube-channel-analysis
   ```

2. Create a virtual environment and activate it:
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```

3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
To run this project on Google Colab, follow these steps:

1.Download The .ipynb File saved as "Youtubers(Stand-Up Comedians)- Channel_Analysis.ipynb"

2.Save it in your Google Drive in a new folder and then open it in google colab , make sure to sign in using the same Gmail.

3.Copy the Path of this new folder to export the channel data and video data of zakir khan's videos in the end of the project.

This step is necessary for both the cases either you run it locally or in any notebook - 

4. Obtain a YouTube Data API Key:
   - Go to [Google Cloud Console](https://console.cloud.google.com/).
   - Create a project and enable the YouTube Data API v3.
   - Generate an API key and paste it in the `config.py` file.

## Usage

Once the environment is set up, you can start the analysis by running the `main.py` script / "Youtubers(Stand-Up Comedians)- Channel_Analysis.ipynb". It will fetch the channel data, perform EDA, generate visualizations, and export the data.

Run the following command:
```bash
python main.py
```

The script will:
- Fetch data from the YouTube API for several comedians.
- Perform exploratory analysis on the channel and video data.
- Visualize the results.
- Save the data in CSV files for later use.

## Data Analysis

The analysis is split into two main parts:

### 1. Channel Data:
- The program fetches channel data for 8 stand-up comedians.
- Key metrics like the number of views, subscribers, total videos, and channel age are collected.
- **Correlations** between these metrics are explored using pandas.

### 2. Zakir Khan's Video Data:
- The program specifically fetches data for Zakir Khan, the most subscribed comedian.
- All videos uploaded by Zakir Khan are analyzed.
- Detailed EDA is performed on features like video views, likes, comments, and video age.

## Visualization

We used **Matplotlib** and **Seaborn** libraries for data visualization. The following types of visualizations are created:

- **Channel Data Visualization**:
  - Correlation heatmaps to visualize relationships between views, subscribers, total videos, and channel age.
  - Bar plots and scatter plots to compare different comedians’ performance.

- **Zakir Khan's Video Data Visualization**:
  - Distribution of views, likes, and comments per video.
  - Visualizations based on total videos uploaded each month and top 10 videos with most views.

The visualizations are displayed using `matplotlib.pyplot` and `seaborn` to generate insightful and easily interpretable charts.

## Data Export

All the fetched data, including:
1. **Channel Data** of 8 stand-up comedians (including views, subscribers, videos, etc.).
2. **Video Details** of Zakir Khan's uploaded videos (including views, likes, comments, etc.).

is exported to CSV files (`channel_data.csv` and `Video_data(zakir khan).csv`). These files can be used for further analysis or to share the data with others.

### Example:
The `channel_data.csv` might look like this:

|   Channel Name  |     Views      |   Subscribers   | Total Videos | Channel Age |
|-----------------|----------------|-----------------|--------------|-------------|
| Zakir Khan      | 799150691      | 4088394         | 300          |      5      |
| Samay Raina     | 924600635      | 3874843         | 200          |      4      |

The `Video_data(zakir khan).csv` might look like this:

| Video Title             |    Views   |   Likes  | Comments |   Month    |
|-------------------------|------------|----------|----------|------------|
| Video 1                 |  20482778  | 50483    | 500      |     May    |
| Video 2                 |  1837723   | 30643    | 300      |   January  |

## Contributing

Contributions to this project are welcome. If you'd like to contribute, please fork the repository, create a new branch, and submit a pull request with your changes.

1. Fork the repository
2. Create a new branch (`git checkout -b feature-branch`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature-branch`)
5. Create a new pull request

## Google Collab Link for project - 

https://colab.research.google.com/drive/1p5sk5FNE369IXA_IMqhd2UQ7WigsqEH0?usp=drive_link

## Folder Link for Project - 

https://drive.google.com/drive/folders/13APZpn9JP5WIi8lgTAXWmSwujoHt5fft?usp=sharing

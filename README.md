# Markdown to Google Docs API Integration

## Overview
This Python script automates the conversion of Markdown meeting notes into structured Google Documents. It utilizes the Google Docs REST API to apply hierarchical formatting, specialized styling for assignees, and checkbox conversions.

## Requirements
The following libraries are required (standard in Google Colab):
- `google-api-python-client`
- `google-auth`

## Setup Instructions
1. Open the provided `.ipynb` notebook in **Google Colab**.
2. Run the script cell. 
3. Follow the Google OAuth prompt to authorize the script to create a document in your Google Drive.
4. Once completed, a link to the formatted Google Doc will be printed in the console.

## Features
- **Header Mapping:** Converts `#`, `##`, `###` to GDoc Headings 1, 2, and 3.
- **Assignee Styling:** Automatically detects `@names` and styles them in **Bold Orchid**.
- **Action Items:** Converts Markdown syntax `- [ ]` into visual checkboxes.
- **Footer Formatting:** Styles meeting metadata in italics.

# Analyzing-Library-Book-Data-Dashboard

## Project Overview

This repository contains a Power BI dashboard project that analyzes library book data to generate insights on borrowing patterns, genre popularity, author performance, and book ratings. The project follows a structured approach to data transformation, visualization, and report publishing as specified in the assignment requirements.

## Dataset Description

The analysis is performed on a single-table dataset called `LibraryBooks` with the following structure:
- **BookID**: Unique identifier for each book
- **Title**: The title of the book
- **Author**: The author of the book
- **Genre**: The genre or category of the book
- **PublishedYear**: The year the book was published
- **CopiesAvailable**: The number of copies of the book currently available in the library
- **TimesBorrowed**: The number of times the book has been borrowed
- **AverageRating**: The average rating of the book given by members

## Features and Implementations

### Data Transformation

- Duplicate removal to ensure data integrity
- Filtering to focus on books published after 2000
- Creation of a `BorrowingFrequency` calculated column using DAX: `BorrowingFrequency = [TimesBorrowed] / (YEAR(TODAY()) - [PublishedYear] + 1)`

### Visualizations

The dashboard contains multiple visualizations across three pages:

#### Page 1: Overview

- Bar chart showing Top 10 Authors based on total borrowing frequency
- Pie chart displaying distribution of books across different genres
- Genre slicer for interactive filtering

#### Page 2: Trends

- Line chart showing the publication trend of books over years
- Year-by-year analysis of the library's collection growth

#### Page 3: Ratings Analysis

- Scatter chart exploring the relationship between average ratings and borrowing frequency
- Insights into reader preferences and book popularity

### Interactive Features

- Cross-filtering capabilities between all visualizations
- Genre slicer for filtering all visualizations simultaneously
- Interactive elements allowing users to explore specific data points

## Implementation Process

1. Data import and initial exploration
2. Data cleaning and transformation using Power Query
3. Creation of calculated measures and columns using DAX
4. Development of visualizations according to specific requirements
5. Implementation of interactivity and filters
6. Report formatting and design optimization
7. Multi-page report creation and organization

## Screenshots

[Include 2-3 screenshots of your dashboard here]

## Tools and Technologies
- **Power BI Desktop**: For dashboard development
- **Power Query**: For data transformation
- **DAX**: For creating calculated columns and measures

## Future Enhancements

- Integration with additional data sources like publisher information
- Creation of more advanced forecasting models for book borrowing trends
- Implementation of bookmark features for different analytical perspectives

## How to Use

1. Download the `.pbix` file from this repository
2. Open the file using Power BI Desktop
3. Explore the interactive visualizations across the three report pages
4. Use the slicer to filter data by genre

## References
- [Power BI Documentation](https://docs.microsoft.com/en-us/power-bi/)
- [DAX Function Reference](https://docs.microsoft.com/en-us/dax/dax-function-reference)

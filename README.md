# London GitHub Users Analysis

- **Data Collection**: The GitHub API was used to collect profiles and repositories for users in London with over 500 followers.
- **Key Insight**: Most users work in popular languages like Python and JavaScript, with a high proportion working at well-known tech companies.
- **Recommendation**: Developers can gain visibility by enhancing README files and adding useful project documentation, which tends to attract more stars and watchers.

## Project Overview
This project scrapes GitHub for data on London-based users with over 500 followers, then analyzes the users and their repositories. The analysis sheds light on trends, user demographics, and development patterns.

### Data Files
- **users.csv**: Contains user profile information, such as login ID, full name, company, location, and more.
- **repositories.csv**: Lists repository details including the full name, star count, main language, and license type.

### Methodology
1. **Data Extraction**: We used the GitHub API to search for users in London with followers exceeding 500. For each user, we fetched up to 500 of their most recent public repositories.
2. **Data Cleaning**: Company names were trimmed, leading `@` symbols were removed, and all names were converted to uppercase. Null values were kept as empty strings for uniformity.
3. **Data Analysis**: Using the CSV data, we performed a range of analyses to gain insights into programming language popularity, company affiliations, and repository usage patterns.

### Key Findings
- **Top Followers**: The users with the highest followers tend to be Python and JavaScript developers.
- **License Trends**: MIT and Apache licenses are among the most popular among these users.
- **Company Representation**: Many users work at well-known tech companies, with some of the most represented being Google and Microsoft.

### Analysis Results
We conducted statistical analysis to answer various questions, including:
- Identifying the most common programming languages.
- Measuring correlation between followers and public repositories.
- Evaluating whether hireable users share emails more frequently.

### Repository Structure
```plaintext
|-- users.csv               # User profile data from GitHub
|-- repositories.csv        # Repository data from GitHub users
|-- README.md               # Project overview and key insights

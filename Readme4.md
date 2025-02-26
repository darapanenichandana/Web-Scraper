# Bing Search Scraper

This Python script performs a web search using Bing and extracts the top 5 search results, displaying them in a structured format using **Pandas**.

## Features
- Sends a search query to **Bing** and retrieves results.
- Parses the search results using **BeautifulSoup**.
- Extracts the **title, link, and description** of each result.
- Stores the results in a **Pandas DataFrame** for easy readability.

## Requirements
Ensure you have the following Python libraries installed:

```bash
pip install requests beautifulsoup4 pandas
```

## Usage
1. Import the function into your Python script or run it directly.
2. Modify the `query` variable with your desired search term.
3. The script will print and return the search results in a Pandas DataFrame.

### Example
```python
query = "recent sports"
df_results = search(query)

if df_results is not None:
    print(df_results)
```

## Output Format
| Title | Link | Description |
|--------|------|-------------|
| Example Title | example.com | Short description of the result |

## Limitations
- The script scrapes Bing's HTML structure, which may change over time.
- Web scraping may violate **Bing's Terms of Service**; consider using the **Bing Search API** for reliable results.

## License
This project is licensed under the **MIT License** – feel free to modify and distribute it.


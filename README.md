# Static Web Page Scraping - Wikipedia Article Navigator
## Wikipedia Programming Language Scraper

This is a command-line tool written in Python that scrapes Wikipedia articles for information about a specified programming language. It demonstrates fundamental web scraping techniques using the `requests` and `BeautifulSoup` libraries.

## Features ✨

-   **Fetch by Language Name**: Simply provide a programming language name, and the script constructs the correct Wikipedia URL.
-   **Comprehensive Data Extraction**: Scrapes key information from the article, including:
    -   The main title.
    -   The first introductory paragraph.
    -   All subheadings (`h2`, `h3`, `h4`, etc.).
    -   All links from the "External links" section.
-   **Interactive Navigation**: Extracts all internal links from the "See also" section and prompts the user to choose one to "follow." If a link is chosen, the script will then scrape the title and first paragraph of that new page.

## How to Use 🚀

1.  **Clone the repository**:
    ```bash
    git clone <your-repo-url>
    cd <your-repo-directory>
    ```

2.  **Install dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

3.  **Run the script from your terminal**:
    The script requires one argument: `-p` or `--programming-language`.

    ```bash
    # Example for Python
    python wiki_scraper.py -p "Python"

    # Example for C++
    python wiki_scraper.py --programming-language "C++"
    ```

## Dependencies 📦

-   `requests`
-   `beautifulsoup4`

## Key Concepts Demonstrated

-   **Argument Parsing**: Using the `argparse` module to create a user-friendly command-line interface.
-   **Static Page Scraping**: Fetching and parsing predictable HTML content from a static website.
-   **HTML Navigation**: Using BeautifulSoup methods like `find()`, `find_all()`, and `find_next()` to locate specific elements based on IDs, tags, and relational position.
-   **Interactive Scripting**: Taking user input to create a dynamic and interactive experience.
-   **Code Modularity**: Creating a reusable function to handle the scraping of "followed" links, avoiding code duplication.

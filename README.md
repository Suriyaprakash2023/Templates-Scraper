# Template Scraper

A Python script to scrape HTML templates, including associated CSS, JavaScript, and images, from a specified URL. The script works only with URLs that end in `.html` (e.g., `https://html.themeholy.com/tourm/demo/home-travel.html`).

## Features

- Scrapes HTML templates along with their CSS, JS, and images.
- Saves the template to a specified folder on your system.

## Prerequisites

- Python 3.7 or higher
- Required Python packages:
  - `requests`
  - `beautifulsoup4`
  - `os`
  - `shutil`

Install the required packages using:

```bash
pip install requests beautifulsoup4
```

## How to Use

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/template-scraper.git
   cd template-scraper
   ```

2. Open the Python script and set the following variables:

   - `base_url`: Replace with the URL you want to scrape. Ensure the URL ends with `.html`.
   - `save_path`: Replace with the directory where you want to save the scraped template.

   Example configuration:

   ```python
   if __name__ == "__main__":
       base_url = 'https://html.themeholy.com/tourm/demo/home-travel.html'  # Replace with the URL you want to scrape
       save_path = 'G:/Template Scrapping/tour'  # Replace with your desired save path
   ```

3. Run the script:

   ```bash
   python scraper.py
   ```

4. The script will start scraping and save the template to the specified folder. Once completed, you will find the full template, including the HTML, CSS, JS, and images, in the target directory.

## Example Output Structure

After scraping, the directory structure will look like this:

```
G:/Template Scrapping/tour/
├── home-travel.html
├── css/
│   ├── style.css
│   └── ...
├── js/
│   ├── script.js
│   └── ...
└── images/
    ├── logo.png
    └── ...
```

## Notes

- Ensure the URL ends with `.html`; otherwise, the script will not proceed.
- Check your internet connection to ensure smooth scraping.
- The script only works with publicly accessible URLs and may not handle dynamically loaded content.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

Feel free to contribute to the project or report issues!

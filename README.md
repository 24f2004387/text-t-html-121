# Static Web App

## Summary
This static web app allows users to load Markdown content from a specified URL using the `?url=` query parameter. If the parameter is not provided, the app defaults to loading the Markdown from an attached file. The active source of the Markdown is displayed in the `#markdown-source-label` element.

## Setup (Local)
To set up the project locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/24f2004387/text-t-html-121.git
   ```
2. Navigate to the project directory:
   ```bash
   cd text-t-html-121
   ```
3. Open `index.html` in your preferred web browser.

## Usage
To use the app, you can either:
- Load a Markdown file directly by accessing the app at `http://localhost/path/to/index.html`.
- Specify a URL to load Markdown content by appending `?url=YOUR_MARKDOWN_URL` to the URL.

The active source will be displayed in the `#markdown-source-label`.

## Code Explanation
The app utilizes JavaScript to fetch Markdown content. It checks for the presence of the `?url=` parameter and uses the Fetch API to retrieve the content if available. The code includes the following key checks:
- The length of `#markdown-source-label` ensures that a source is displayed.
- The presence of `fetch(` in the script confirms that the app is set up to load external content.

## Deployment (GitHub Pages)
To deploy the app using GitHub Pages, follow these steps:

1. Push your changes to the `main` branch of your repository.
2. Go to the repository settings on GitHub.
3. Under the "Pages" section, select the `main` branch as the source.
4. Your app will be available at `https://<username>.github.io/<repository-name>/`.

For this project, the live URL is: [https://24f2004387.github.io/text-t-html-121/](https://24f2004387.github.io/text-t-html-121/)

## License (MIT)
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
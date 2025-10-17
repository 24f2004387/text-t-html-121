# Static Web App

## Summary
This static web app allows users to load and display Markdown content from a specified URL using a `?url=` query parameter. If the parameter is not provided, the app falls back to loading a default Markdown attachment. The active source of the displayed content is indicated in the `#markdown-source-label`.

## Setup (Local)
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/static-web-app.git
   ```
2. Navigate to the project directory:
   ```bash
   cd static-web-app
   ```
3. Open `index.html` in your preferred web browser.

## Usage
To use the app, simply append a `?url=` parameter to the URL in your browser. For example:
```
http://localhost/static-web-app/index.html?url=https://example.com/sample.md
```
If no URL is provided, the app will load the default Markdown file.

## Code Explanation
- The app checks for the presence of a `?url=` parameter in the URL.
- If present, it fetches the Markdown content using the Fetch API and displays it.
- The active source is displayed in the `#markdown-source-label` element.
- Evaluation checks ensure that the source label is populated and that the Fetch API is used for loading content.

## Deployment (GitHub Pages)
1. Push your code to the `main` branch of your GitHub repository.
2. Navigate to the repository settings.
3. Under the "Pages" section, select the `main` branch as the source.
4. Your app will be available at `https://yourusername.github.io/static-web-app`.

## License (MIT)
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
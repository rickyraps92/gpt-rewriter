## RSS Feed to Blog Article Converter

This Python script allows you to fetch and parse articles from multiple RSS feeds, generate prompts, and utilize OpenAI's GPT-3.5 Turbo model to create blog articles, SEO descriptions, and social media posts. The generated content is then saved as Word documents.

### Setup

1. Make sure you have Python installed on your system.
2. Install the required Python packages by running the following command:

   ```
   pip install python-docx requests beautifulsoup4 openai feedparser python-dateutil pytz
   ```

3. Obtain an API key from OpenAI. Replace `"YOUR_OPENAI_API_KEY"` in the code with your actual API key.

### Usage

1. Edit the `rss_urls` list in the script to include the RSS feeds you want to fetch articles from.
2. Customize the prompt text in the `prompt_start` variable according to your requirements.
3. Run the script using the following command:

   ```
   python gpt_rewriter.py
   ```

4. The script will fetch the RSS feeds, filter the entries from the last 24 hours, and process each entry.
5. For each entry, the script will fetch the webpage content, create a prompt combining the content and the predefined prompt text, and send it to GPT-3.5 Turbo for rewriting.
6. The generated article will be saved as a Word document, with the filename derived from the response content.
7. The URL of the original article will be included at the end of the generated document.

Please ensure you comply with OpenAI's usage policies and guidelines when using their models.

Feel free to modify the script to suit your specific needs. You can explore additional functionality such as error handling, formatting options, or integrating with other tools or platforms.

If you have any questions or need assistance, please don't hesitate to reach out.

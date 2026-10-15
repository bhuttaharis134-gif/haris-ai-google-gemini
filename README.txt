HARIS AI — Google Gemini API version

FILES
- index.html: chat interface; saves chats in the current browser only
- api.php: PHP backend calls Google's Gemini generateContent API
- config.example.php: template for the secret configuration
- README.txt: setup instructions

SETUP
1. Get a Gemini API key from Google AI Studio: https://aistudio.google.com/app/apikey
2. Copy config.example.php and rename the copy to config.php.
3. Open config.php in Sublime Text. Replace PASTE_YOUR_GEMINI_API_KEY_HERE with your own key. Do not send the key to anyone.
4. Upload index.html, api.php, and config.php to the same folder on PHP hosting.
5. Open the website using its hosting URL (https://your-domain/), NOT by double-clicking index.html / file://.
6. Send a test message.

FREE TIER / MODEL
Gemini API free-tier availability, quotas, and eligible models depend on Google AI Studio/account terms and may change. Check the official AI Studio usage page. If gemini-2.5-flash is unavailable to your account, choose a currently available model and update the model value in config.php.

IMPORTANT
- The PHP host must support PHP 8+, cURL, and outbound HTTPS to generativelanguage.googleapis.com.
- Some free shared hosting services block outbound API requests. If so, use a host that permits outbound HTTPS/API calls.
- This is not ChatGPT's private model/backend; it is a separate Gemini-powered assistant with a similar chat interface.
- This starter has no secure user authentication, database-backed history, rate limiting, or payments. Upgrade is only a placeholder.
- Do not publish config.php in public repositories or share your API key.

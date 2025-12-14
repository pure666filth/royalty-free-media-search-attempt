# API Setup Guide

This guide will help you set up the API keys needed for the Royalty-Free Media Search application.

## Overview

The application integrates with three major royalty-free media platforms:
- **Unsplash** - High-quality photos
- **Pexels** - Photos and videos
- **Pixabay** - Photos, videos, and illustrations

## Getting API Keys

### 1. Unsplash API Key

1. Go to [Unsplash Developers](https://unsplash.com/developers)
2. Click "Register as a developer"
3. Create a new application
4. Fill in the application details:
   - Application name: "Royalty-Free Media Search"
   - Description: "A web application to search for royalty-free media"
5. Accept the API terms
6. Copy your **Access Key** (this is your API key)

**Rate Limits:** 50 requests per hour (Demo), 5000 requests per hour (Production)

### 2. Pexels API Key

1. Go to [Pexels API](https://www.pexels.com/api/)
2. Click "Get Started"
3. Sign up or log in to your account
4. Fill in the API request form:
   - Project name: "Royalty-Free Media Search"
   - Project description: "A web application to search for royalty-free media"
5. Your API key will be displayed immediately
6. Copy your **API Key**

**Rate Limits:** 200 requests per hour, 20,000 requests per month

### 3. Pixabay API Key

1. Go to [Pixabay API Documentation](https://pixabay.com/api/docs/)
2. Click "Get Started" or scroll to the registration section
3. Sign up or log in to your account
4. Navigate to the API section in your account settings
5. Copy your **API Key**

**Rate Limits:** 5,000 requests per hour, 100 requests per minute

## Adding API Keys to the Application

### Method 1: Direct Edit (Recommended for local use)

1. Open `index.html` in a text editor
2. Find the `API_KEYS` object in the JavaScript section (around line 500):

```javascript
const API_KEYS = {
    unsplash: '', // Add your Unsplash API key here
    pexels: '', // Add your Pexels API key here
    pixabay: '' // Add your Pixabay API key here
};
```

3. Replace the empty strings with your actual API keys:

```javascript
const API_KEYS = {
    unsplash: 'YOUR_UNSPLASH_ACCESS_KEY',
    pexels: 'YOUR_PEXELS_API_KEY',
    pixabay: 'YOUR_PIXABAY_API_KEY'
};
```

4. Save the file

### Method 2: Environment Variables (Recommended for production)

For production deployments, it's better to use environment variables or a backend proxy to keep your API keys secure.

**Important Security Notes:**
- Never commit API keys to public repositories
- Consider using a backend proxy for production applications
- Add `index.html` to `.gitignore` if it contains API keys
- Use environment variables in production environments

## Testing Your Setup

1. Open `index.html` in a web browser
2. The default search for "nature" should automatically run
3. You should see results from the configured APIs
4. If you see an error message, check:
   - API keys are correctly copied (no extra spaces)
   - API keys are active and not expired
   - You haven't exceeded rate limits

## Rate Limit Management

To avoid hitting rate limits:

1. **Cache Results**: Store search results temporarily
2. **Debounce Searches**: Wait for user to finish typing before searching
3. **Limit Concurrent Requests**: Don't search all APIs simultaneously for every query
4. **Use Pagination**: Load results in batches

## Troubleshooting

### "No API keys configured" Error
- Make sure you've added at least one API key
- Check that the API key is in the correct format
- Verify there are no extra spaces or quotes

### "API Error" Messages
- Check your API key is valid and active
- Verify you haven't exceeded rate limits
- Check your internet connection
- Try the API key in the provider's API documentation

### No Results Found
- Try different search terms
- Check if the API is working by testing directly on the provider's website
- Verify your API key has the correct permissions

## API Documentation Links

- [Unsplash API Docs](https://unsplash.com/documentation)
- [Pexels API Docs](https://www.pexels.com/api/documentation/)
- [Pixabay API Docs](https://pixabay.com/api/docs/)

## License Information

All three platforms provide royalty-free media with generous licenses:

- **Unsplash**: Free to use for commercial and non-commercial purposes
- **Pexels**: Free to use for commercial and non-commercial purposes
- **Pixabay**: Free to use for commercial and non-commercial purposes

Always check the specific license terms on each platform for the most up-to-date information.

## Support

If you encounter issues:
1. Check the API provider's status page
2. Review the API documentation
3. Check the browser console for error messages
4. Verify your API keys are correct and active
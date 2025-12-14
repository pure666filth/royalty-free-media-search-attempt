# Royalty-Free Media Search Engine

A modern web application for searching royalty-free images and videos from multiple sources including Unsplash, Pexels, and Pixabay.

## Features

✨ **Real API Integration**
- Search across Unsplash, Pexels, and Pixabay simultaneously
- Real-time results from multiple sources
- Support for both images and videos

🎨 **Modern UI/UX**
- Clean, responsive design
- Smooth animations and transitions
- Mobile-friendly interface
- Modal view for detailed media information

🔍 **Advanced Search & Filtering**
- Search by keywords
- Filter by media type (images/videos)
- Filter by source (Unsplash/Pexels/Pixabay)
- Pagination for easy browsing

⚡ **Performance Features**
- Parallel API requests for faster results
- Loading states and error handling
- Optimized image loading with lazy loading
- Smooth pagination

📥 **Download & Share**
- Direct download links to high-quality media
- View source links to original content
- Author attribution and licensing information

## Setup

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- API keys from Unsplash, Pexels, and Pixabay (free to obtain)

### Getting API Keys

1. **Unsplash**: [Get API Key](https://unsplash.com/developers)
2. **Pexels**: [Get API Key](https://www.pexels.com/api/)
3. **Pixabay**: [Get API Key](https://pixabay.com/api/docs/)

See [API_SETUP.md](API_SETUP.md) for detailed instructions.

### Installation

1. Clone this repository:
```bash
git clone https://github.com/pure666filth/royalty-free-media-search-attempt.git
cd royalty-free-media-search-attempt
```

2. Open `index.html` in a text editor

3. Add your API keys to the `API_KEYS` object:
```javascript
const API_KEYS = {
    unsplash: 'YOUR_UNSPLASH_ACCESS_KEY',
    pexels: 'YOUR_PEXELS_API_KEY',
    pixabay: 'YOUR_PIXABAY_API_KEY'
};
```

4. Open `index.html` in your web browser

## Usage

1. Enter a search term in the search box
2. Select media type (All/Images/Videos)
3. Choose a source or search all sources
4. Click "Search" or press Enter
5. Browse results and click on any item for details
6. Download or view source from the detail modal

## Features Implemented

### ✅ Fixed Issues
- ✅ Real API integration (no more mock data)
- ✅ Actual search functionality with live results
- ✅ Error handling and user feedback
- ✅ Loading states during API calls
- ✅ Working download functionality
- ✅ Source attribution and licensing info
- ✅ Multi-source filtering
- ✅ Responsive design improvements

### 🎯 Key Improvements
- Parallel API requests for faster results
- Better error messages and user guidance
- Clean, modern UI with smooth animations
- Proper pagination with page numbers
- Modal view for detailed media information
- Direct links to download and source pages

## Technologies Used

- HTML5
- CSS3 (with animations and gradients)
- Vanilla JavaScript (ES6+)
- Unsplash API
- Pexels API
- Pixabay API

## License Information

All media from the integrated sources is royalty-free:
- **Unsplash**: Free to use for commercial and non-commercial purposes
- **Pexels**: Free to use for commercial and non-commercial purposes
- **Pixabay**: Free to use for commercial and non-commercial purposes

Always verify the specific license terms on each platform.

## Contributing

Suggestions and contributions are welcome! Feel free to:
- Open issues for bugs or feature requests
- Submit pull requests with improvements
- Share feedback on the UI/UX

## Roadmap

Future improvements planned:
- [ ] Backend proxy for API key security
- [ ] User favorites/bookmarking system
- [ ] Advanced filters (color, orientation, size)
- [ ] Search history
- [ ] Batch download functionality
- [ ] Collections/boards feature

## Support

If you encounter issues:
1. Check [API_SETUP.md](API_SETUP.md) for setup instructions
2. Verify your API keys are correct and active
3. Check the browser console for error messages
4. Open an issue on GitHub

## Acknowledgments

- [Unsplash](https://unsplash.com) for their amazing photo API
- [Pexels](https://www.pexels.com) for free stock photos and videos
- [Pixabay](https://pixabay.com) for their extensive media library

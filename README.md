# TikTok Content Labeling Tool v2.2

A professional TikTok content labeling tool with modern interface and advanced features.

## 🚀 Key Features

### ✨ Modern Interface
- **Glassmorphism Design**: Transparent interface with modern blur effects
- **Responsive Design**: Compatible with all devices
- **Dark Mode Support**: Built-in dark mode toggle
- **Smooth Animations**: Fluid motion effects and transitions

### 🎯 Labeling Features
- **Multi-label Support**: Apply multiple labels to a single video
- **Smart Video Loading**: Automatically tries different video embedding methods
- **Real-time Progress**: Track labeling progress in real-time
- **Auto-save**: Automatic data saving with backup system
- **Keyboard Shortcuts**: Quick labeling with keyboard shortcuts

### 📊 Data Management
- **CSV Import/Export**: Full CSV support with flexible format
- **Sample File Support**: Built-in sample file for testing
- **Local Storage**: Temporary storage in browser
- **Backup System**: Automatic backup system
- **Data Validation**: Comprehensive data integrity checks

## 📁 File Structure

```
tiktok-labeling-tool/
├── index.html          # Main HTML file
├── styles.css          # Main CSS styles
├── Guideline.csv       # Labeling guidelines data
├── 100samples.csv      # Sample data file
└── README.md           # This documentation
```

## 🛠️ How to Use

### 1. Prepare Data
- CSV file needs `username` and `id_video` columns (required)
- Other columns will be automatically created with default values
- Optional: Include all columns for pre-labeled data

### 2. Using the Tool
1. **Choose Data Source**: 
   - Use sample file for testing
   - Upload your own CSV file
2. **View Videos**: Select videos from the list
3. **Apply Labels**: Choose appropriate labels
4. **Export Results**: Download labeled CSV file

### 3. Video Embedding Methods
- **🎯 Smart Auto**: Automatically tries all methods
- **🎬 oEmbed**: Uses TikTok oEmbed API
- **📺 Blockquote**: Native embedding method
- **🔗 External**: Direct link to TikTok

## 🎨 Design System

### Color Palette
```css
--primary-color: hsl(220, 100%, 60%)    /* Primary Blue */
--secondary-color: hsl(280, 70%, 70%)   /* Secondary Purple */
--accent-color: hsl(350, 85%, 70%)      /* Accent Pink */
--success-color: hsl(142, 76%, 60%)     /* Success Green */
--warning-color: hsl(45, 95%, 80%)      /* Warning Yellow */
--error-color: hsl(348, 86%, 80%)       /* Error Red */
```

### Typography
- **Primary Font**: Inter (Google Fonts)
- **Code Font**: JetBrains Mono
- **Responsive**: Automatic size adjustment

### Spacing System
```css
--space-xs: 0.25rem    /* 4px */
--space-sm: 0.5rem     /* 8px */
--space-md: 1rem       /* 16px */
--space-lg: 1.5rem     /* 24px */
--space-xl: 2rem       /* 32px */
```

## 🔧 Technical Features

### Video Loading System
- **Parallel Loading**: Load multiple methods simultaneously
- **Caching**: Cache results for improved performance
- **Fallback**: Automatic fallback to alternative methods
- **Error Handling**: Comprehensive error management

### Data Management
- **Flexible CSV Format**: Supports minimal (username, id_video) and full formats
- **Auto-column Generation**: Automatically creates missing columns
- **Data Validation**: Ensures data integrity
- **Backup Rotation**: Maintains recent backups

### Performance Optimizations
- **Lazy Loading**: Load videos on demand
- **Debouncing**: Prevent excessive API calls
- **Memory Management**: Automatic memory cleanup
- **Efficient Rendering**: Optimized DOM updates

## 📱 Responsive Design

### Breakpoints
- **Desktop**: > 1200px
- **Tablet**: 768px - 1200px
- **Mobile**: < 768px

### Mobile Optimizations
- Touch-friendly buttons
- Swipe gestures
- Optimized video player
- Simplified navigation

## 🔒 Security & Privacy

- **Local Processing**: All data processed locally
- **No Server**: No data sent to external servers
- **File System Access**: Uses File System Access API (when available)
- **Sample Mode**: Test mode with temporary storage only

## 🎯 Labeling Categories

### Content Types
- **Safe**: Appropriate content for all audiences
- **Harmful Content**: Content that may cause harm
- **Suicide**: Content related to self-harm or suicide
- **Adult Content**: Mature content not suitable for minors
- **Confuse**: Content that's unclear or ambiguous
- **Empty**: Unavailable or non-functional content

### Labeling Guidelines
- Each video can have one primary label
- Multiple secondary labels allowed
- Automatic validation of label combinations
- Real-time feedback on labeling progress

## 🚀 Advanced Features

### Keyboard Shortcuts
- **Ctrl+1**: Harmful Content
- **Ctrl+2**: Suicide
- **Ctrl+3**: Adult Content
- **Ctrl+4**: Safe
- **Ctrl+5**: Confuse
- **Ctrl+6**: Empty
- **Ctrl+S**: Export CSV
- **←/→**: Navigate videos

### Auto-save System
- Automatic saving every 5 minutes
- Buffer-based saving for efficiency
- Backup system with multiple versions
- Data integrity validation

### Export Options
- **Sample Mode**: Downloads as `sample_test_results_[timestamp].csv`
- **Real File Mode**: Downloads as `labeled_tiktok_videos_[timestamp].csv`
- **Full Format**: Includes all columns in standard order
- **Compatible**: Works with existing labeling workflows

## 🐛 Troubleshooting

### Video Not Displaying
1. Check internet connection
2. Try different embedding methods
3. Verify video URL validity
4. Check browser console for errors

### CORS Errors
- These are normal TikTok-related errors
- Don't affect labeling functionality
- Can be safely ignored

### Data Loss Issues
1. Check localStorage
2. Try backup restoration
3. Verify browser storage capacity
4. Check for browser updates

### CSV Import Issues
1. Ensure required columns (username, id_video) are present
2. Check CSV format (UTF-8 encoding)
3. Verify no special characters in headers
4. Try with sample file first

## 🔮 Future Roadmap

### Upcoming Features
- [ ] Batch processing capabilities
- [ ] AI-assisted labeling
- [ ] Export to multiple formats (JSON, XML)
- [ ] Collaborative labeling
- [ ] Advanced analytics dashboard
- [ ] Custom label categories
- [ ] Bulk video import
- [ ] Label confidence scoring

### Technical Improvements
- [ ] Service Worker for offline support
- [ ] WebAssembly for better performance
- [ ] IndexedDB for larger datasets
- [ ] WebRTC for real-time collaboration
- [ ] Progressive Web App (PWA) features
- [ ] Advanced caching strategies

## 📄 License

MIT License - See LICENSE file for details.

## 🤝 Contributing

All contributions are welcome! Please:

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

### Development Guidelines
- Follow existing code style
- Add comments for complex logic
- Test on multiple browsers
- Update documentation as needed

## 📞 Contact & Support

- **Issues**: [GitHub Issues](https://github.com/your-repo/issues)
- **Discussions**: [GitHub Discussions](https://github.com/your-repo/discussions)
- **Email**: [your-email@example.com]

## 🙏 Acknowledgments

- TikTok for providing video embedding APIs
- The open-source community for various libraries
- Contributors and testers who helped improve the tool

---

**Made with ❤️ for the TikTok research community**

*This tool is designed to help researchers and content moderators efficiently label TikTok content for analysis and research purposes.* 
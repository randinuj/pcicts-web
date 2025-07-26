# PCICTS Website

The official website for President's College Information & Communication Technology Society (PCICTS).

## About

This website showcases the activities, projects, achievements, and team members of the PCICTS. It features a modern, responsive design with glassmorphism effects and smooth animations.

## Features

- **Responsive Design**: Optimized for all devices and screen sizes
- **Modern UI**: Glassmorphism design with smooth animations
- **Team Showcase**: Display of board members and their roles
- **Project Gallery**: Showcase of ongoing and completed projects
- **Achievements Section**: Highlighting society accomplishments
- **Contact Information**: Easy access to contact details
- **NovaQuest Event Page**: Dedicated page for the annual quiz competition

## File Structure

```
pcicts-web/
├── index.html                 # Main homepage
├── novaquest.html            # NovaQuest event page
├── history.html              # Society history page
├── blog_article_page_template.html  # Blog template
├── project_page_template.html       # Project template
├── assets/
│   ├── css/
│   │   ├── style.css         # Main stylesheet
│   │   └── style-novaquest.css # NovaQuest specific styles
│   ├── images/
│   │   ├── *.jpg             # Team member photos
│   │   ├── *.png             # Logos and graphics
│   └── fonts/
│       ├── Squartiqa4F.woff  # Custom font files
│       └── Squartiqa4F.woff2
└── README.md                 # This file
```

## Technologies Used

- **HTML5**: Semantic markup
- **CSS3**: Modern styling with CSS Grid, Flexbox, and custom properties
- **JavaScript**: Interactive features and animations
- **Font Awesome**: Icons
- **Google Fonts**: Product Sans font family

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## Setup and Deployment

### Local Development

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/pcicts-web.git
   cd pcicts-web
   ```

2. Open `index.html` in your web browser or use a local server:
   ```bash
   # Using Python
   python -m http.server 8000
   
   # Using Node.js
   npx serve .
   ```

3. Visit `http://localhost:8000` in your browser

### Deployment

The website is ready for deployment on any static hosting service:

- **GitHub Pages**: Push to a GitHub repository and enable Pages
- **Netlify**: Drag and drop the folder or connect to Git repository
- **Vercel**: Import the repository
- **Firebase Hosting**: Use Firebase CLI to deploy

## Customization

### Colors
The color scheme is defined using CSS custom properties in `assets/css/style.css`:

```css
:root {
    --primary-color: #3b82f6;
    --bg-primary: #000000;
    --text-primary: #ffffff;
    /* ... more variables */
}
```

### Content
- Update team member information in `index.html`
- Modify project details in the projects section
- Add new achievements as needed
- Update contact information

## Performance Optimizations

- Images are optimized and organized in the `assets/images/` directory
- Font files are in modern formats (WOFF2, WOFF)
- CSS is minified and organized
- JavaScript is optimized for performance

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## License

This project is maintained by PCICTS. All rights reserved.

## Contact

For questions or support, contact PCICTS through the website or email.

---

**PCICTS** - Empowering students through technology and innovation. 
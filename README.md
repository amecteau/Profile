# Professional Profile

A professional profile and resume website built with GitHub Pages and automated deployment via GitHub Actions.

## 🌟 Features

- **Professional Design**: Clean, responsive design that looks great on all devices
- **Markdown-Based**: Easy to update your profile by editing a simple markdown file
- **Automated Deployment**: GitHub Actions pipeline automatically builds and deploys your site
- **Release Pipeline**: Push to development branch, and changes are automatically promoted to GitHub Pages

## 📋 Setup Instructions

### Initial Setup

1. **Enable GitHub Pages**:
   - Go to your repository Settings → Pages
   - Under "Build and deployment", select "Source: GitHub Actions"
   - Save the settings

2. **Edit Your Profile**:
   - Open `profile.md` and replace the template content with your information
   - Commit and push your changes to the development branch

3. **Automatic Deployment**:
   - The GitHub Actions workflow will automatically trigger on push
   - Your site will be built and deployed to GitHub Pages
   - Access your site at: `https://amecteau.github.io/Profile`

### Customization

#### Update Profile Content

Edit `profile.md` with your information:
- Professional summary
- Work experience
- Education
- Skills
- Projects
- Certifications
- Contact information

#### Customize Styling

Modify `style.css` to change:
- Colors (defined in CSS variables at the top)
- Fonts
- Layout
- Animations

#### Customize Homepage

Edit `index.html` to change:
- Navigation structure
- Hero section content
- Page layout

#### Update Site Configuration

Edit `_config.yml` to update:
- Site title and description
- Author information
- Email address

## 🚀 Deployment Pipeline

This project uses a simple release pipeline approach:

```
Development Branch → GitHub Actions → GitHub Pages (Production)
```

### Workflow

1. **Make Changes**: Edit files on your development branch
2. **Commit & Push**: Push changes to GitHub
3. **Automatic Build**: GitHub Actions workflow triggers automatically
4. **Deploy**: Site is built with Jekyll and deployed to GitHub Pages
5. **Live**: Changes appear on your live site within minutes

### Manual Deployment

You can also manually trigger the deployment:
1. Go to Actions tab in your repository
2. Select "Deploy Profile to GitHub Pages" workflow
3. Click "Run workflow"

## 📁 Project Structure

```
.
├── .github/
│   └── workflows/
│       └── deploy-pages.yml    # GitHub Actions workflow
├── index.html                   # Main HTML page
├── profile.md                   # Your profile content (EDIT THIS!)
├── style.css                    # Styling
├── _config.yml                  # Jekyll configuration
└── README.md                    # This file
```

## 🛠️ Technologies Used

- **GitHub Pages**: Static site hosting
- **Jekyll**: Static site generator
- **GitHub Actions**: CI/CD pipeline
- **Markdown**: Content formatting
- **HTML/CSS**: Frontend structure and styling
- **JavaScript**: Dynamic content loading

## 📝 Usage Guide

### Updating Your Profile

1. **Quick Update**:
   ```bash
   # Edit the profile
   vim profile.md
   
   # Commit and push
   git add profile.md
   git commit -m "Update profile information"
   git push
   ```

2. **The workflow will automatically**:
   - Detect your push
   - Build the site with Jekyll
   - Deploy to GitHub Pages
   - Make your changes live

### Viewing Your Site Locally

To preview your site locally before pushing:

```bash
# Install Jekyll (requires Ruby)
gem install jekyll bundler

# Serve the site locally
jekyll serve

# Visit http://localhost:4000/Profile in your browser
```

## 🎨 Customization Tips

### Change Color Scheme

Edit the CSS variables in `style.css`:

```css
:root {
    --primary-color: #2c3e50;    /* Main navigation/headers */
    --secondary-color: #3498db;  /* Links and accents */
    --accent-color: #e74c3c;     /* Call-to-action buttons */
    --text-color: #333;          /* Main text */
    --light-bg: #ecf0f1;         /* Background */
    --white: #ffffff;            /* White elements */
}
```

### Add New Sections

Add new sections to `profile.md` using markdown:

```markdown
## New Section Name

Your content here...
```

### Modify Navigation

Edit the navigation in `index.html`:

```html
<nav>
    <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#your-section">Your Section</a></li>
    </ul>
</nav>
```

## 🔒 Security

- No sensitive data is stored in the repository
- All deployment is handled securely through GitHub Actions
- GITHUB_TOKEN is automatically provided and secured by GitHub

## 📄 License

This project is open source and available for personal and commercial use.

## 🤝 Contributing

Feel free to fork this repository and customize it for your own use!

## 📧 Support

For issues or questions, please open an issue in the GitHub repository.

---

**Last Updated**: February 2026

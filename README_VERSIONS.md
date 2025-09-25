# Sparse VideoGen - Multi-Version Website Structure

This project now supports multi-version access, allowing you to access different versions of the project page through different URLs.

## Access Links

- **Main Page (Version Selection)**: https://svg-project.github.io/
- **Version 1**: https://svg-project.github.io/v1/
- **Version 2**: https://svg-project.github.io/v2/

## File Structure

```
Project Root/
├── index.html          # Version selection page
├── static/             # Shared static resources
├── assets/             # Shared asset files
├── v1/                 # Complete website for version 1
│   ├── index.html      # v1 main page
│   ├── assets/         # v1 asset files
│   └── static/         # v1 static files
├── v2/                 # Complete website for version 2
│   ├── index.html      # v2 main page
│   ├── assets/         # v2 asset files
│   └── static/         # v2 static files
└── README_VERSIONS.md  # This documentation file
```

## How to Update Versions

### Update v1 Version
1. Edit the `v1/index.html` file
2. Update resource files in `v1/assets/` and `v1/static/`

### Update v2 Version
1. Edit the `v2/index.html` file
2. Update resource files in `v2/assets/` and `v2/static/`

### Add New Version
1. Create a new version folder (e.g., `v3/`)
2. Copy existing version content to the new folder
3. Update the new version content
4. Add new version link in the root `index.html`

## GitHub Pages Setup

Make sure in your GitHub repository settings:
1. GitHub Pages is enabled
2. Source is set to "Deploy from a branch"
3. Branch is selected as "main" (or your main branch)
4. Folder is selected as "/ (root)"

## Local Testing

In Windows environment, you can use the following methods for local testing:

1. Use Python's simple HTTP server:
```bash
python -m http.server 8000
```

2. Then access in your browser:
- http://localhost:8000/ (Version selection page)
- http://localhost:8000/v1/ (Version 1)
- http://localhost:8000/v2/ (Version 2)

## Notes

- Each version is completely independent, containing its own resource files
- The version selection page uses modern CSS design with responsive layout
- All versions maintain their original functionality and styling
- Resource paths are properly configured to ensure each version runs independently

## Customization

You can customize as needed:
- Modify the style and layout of the version selection page
- Set different theme colors for different versions
- Add version-specific features and content
- Customize version descriptions and link text

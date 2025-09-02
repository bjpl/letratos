# Contributing to Letratos

Thank you for your interest in contributing to Letratos!

## Adding New Content

### Adding a New Poem

#### English Poems
1. Create a new markdown file in `_poems_en/`
2. Use the following frontmatter structure:
```yaml
---
layout: poem
title: "Your Poem Title"
date: YYYY-MM-DD
lang: en
---
```
3. Add your poem content below the frontmatter

#### Spanish Poems
1. Create a new markdown file in `_poems_es/`
2. Use the following frontmatter structure:
```yaml
---
layout: poem
title: "Título de tu Poema"
date: YYYY-MM-DD
lang: es
---
```
3. Add your poem content below the frontmatter

### Adding a New Photo Gallery

1. Add your images to a new folder in `assets/images/YourGalleryName/`
2. Create a new markdown file in `_photography/`
3. Use the following frontmatter structure:
```yaml
---
layout: photography
title: "Gallery Name"
date: YYYY-MM-DD
thumbnail: "/assets/images/YourGalleryName/thumbnail.jpg"
images:
  - url: "/assets/images/YourGalleryName/image1.jpg"
    caption: "📍 Location, State/Country"
    alt: "Description of image"
  - url: "/assets/images/YourGalleryName/image2.jpg"
    caption: "📍 Location, State/Country"
    alt: "Description of image"
---
```

## Style Guidelines

### Poetry
- Keep formatting minimal and let the words speak
- Use markdown line breaks (two spaces at end of line) for intentional breaks within stanzas
- Use blank lines to separate stanzas

### Photography
- Use descriptive but concise alt text
- Include location with pin emoji (📍) in captions
- Keep image file sizes reasonable for web (ideally under 2MB)

## Development Workflow

1. Fork the repository
2. Create a feature branch (`git checkout -b add-new-poem`)
3. Make your changes
4. Test locally with `bundle exec jekyll serve`
5. Commit your changes (`git commit -m 'Add new poem: Title'`)
6. Push to your fork (`git push origin add-new-poem`)
7. Create a Pull Request

## Local Testing

Before submitting, ensure:
1. The site builds without errors
2. Your content displays correctly
3. Navigation works properly
4. Images load correctly (for photography)

## Questions?

Feel free to open an issue for any questions or suggestions.
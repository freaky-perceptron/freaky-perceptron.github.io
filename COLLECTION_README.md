# Collection System

This collection system allows you to store and display interesting quotes, writeups, and poems on your personal site.

## How It Works

The collection is powered by Jekyll data files and automatically displays content on the `/collection` page. All collection items are stored in `_data/collection.yml`.

## Adding New Items

### 1. Quotes
```yaml
quotes:
  - text: "Your quote text here"
    author: "Author Name"
    source: "Where you found it (optional)"
    category: "motivation" # optional category
```

### 2. Writeups
```yaml
writeups:
  - title: "Title of your writeup"
    subtitle: "Brief description"
    content: "Your full writeup content here"
    author: "Your name or source"
    date: "2024" # optional
    category: "philosophy" # optional
```

### 3. Poems
```yaml
poems:
  - title: "Poem Title"
    author: "Poet Name"
    content: |
      Your poem content here
      Multiple lines work with the pipe symbol
      Each line will be preserved
    source: "Book or publication (optional)"
    category: "inspiration" # optional
```

## Categories

You can use any categories you like. Some suggestions:
- motivation
- philosophy
- life
- inspiration
- education
- creativity
- choices
- empowerment

## File Structure

```
_data/
  collection.yml          # Main collection data file
collection.html           # Collection page template
_includes/
  navbar.html            # Navigation (updated with Collection link)
```

## Benefits

1. **Easy Management**: Just edit the YAML file to add/remove items
2. **Automatic Updates**: Changes appear immediately when you rebuild the site
3. **Organized**: Items are automatically categorized and displayed
4. **Searchable**: Content is part of your site and can be indexed by search engines
5. **Responsive**: Works on all devices

## Future Enhancements

- Add search functionality
- Filter by category
- Add tags
- Sort by date
- Add pagination for large collections
- Import from external sources

## Tips

- Keep quotes concise and impactful
- Use consistent formatting for writeups
- Preserve line breaks in poems using the pipe symbol (|)
- Add categories to help organize your collection
- Include sources when possible for attribution

# 4th Grade Orange Class  Parent Resources

A simple webpage with quick links for parents and guardians.

## How to Make Changes

All the links are stored in the `index.html` file in a JavaScript array called `links` (starting around line 110).

### Adding a New Link

1. Find the category where you want to add the link (e.g., "Key Resources", "Apps & Tools")
2. Inside that category's `items: [ ]` array, add a new entry like this:

```javascript
{
  icon: 'fa-solid fa-link',
  title: "Your Link Title",
  url: "https://example.com",
  description: "Brief description of what this link does.",
}
```

**Important:** Don't forget the comma after the `}` if there are more items after it!

### Editing an Existing Link

Find the link you want to change and edit its `title`, `url`, or `description`.

### Removing a Link

Find the link and delete the entire `{ ... },` block (including the comma).

### Changing Icons

Icons use [Font Awesome](https://fontawesome.com/icons). To change an icon:
1. Visit fontawesome.com/icons
2. Find an icon you like
3. Copy the class name (e.g., `fa-solid fa-calendar`)
4. Replace the `icon:` value

### Adding a New Category

Add a new object to the `links` array:

```javascript
{
  category: "New Category Name",
  notes: "Optional subtitle or notes.",
  items: [
    // your links here
  ]
},
```

## Common Gotchas

- **Missing commas:** JavaScript needs commas between items in the array. If the page breaks, check for missing commas.
- **Quotes:** Use matching quotes (`"..."` or `'...'`) around text. Don't mix them.
- **Testing changes:** Open `index.html` in a web browser to see your changes. Refresh the page to see updates.

## Questions?

Email Andrea at amldrummond@gmail.com

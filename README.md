## 1. HTML Structure Overview
The provided HTML file is the base structure for your website. It consists of the following main components:
- **Header Section:** Displays the title.
- **Currently Reading Section:** Highlights the book you are currently reading.
- **Search and Filter Section:** Allows users to search and filter through books.
- **Books Container:** Displays your book list.
- **Pagination Section:** Handles navigation between pages of books.
- **Footer Section:** Includes additional information or links.

## 2. Required Files
To ensure the website functions properly, you need the following:

1. **HTML File**: The main file (`index.html`).
2. **Images**: Placeholder or real book images for books you want to display.
3. **Data Files**:
    - `read.json`: Contains details of books you have read.
    - `to-read.json`: Contains details of books you want to read.
    - `reading.json`: Contains details of the book you are currently reading.

## 3. JSON Data Structure
Create JSON files, they could look like this:

### Books Read (`read.json`):
```json
[
  {
    "title": "Book Title",
    "author": "Author Name",
    "dateRead": "YYYY-MM-DD",
    "rating": 4,
    "image": "path/to/image.jpg",
    "review": "Brief review of the book."
  }
]
```

### Books to Read (`to-read.json`):
```json
[
  {
    "title": "Book Title",
    "author": "Author Name",
    "image": "path/to/image.jpg"
  }
]
```

### Currently Reading (`reading.json`):
```json
{
  "title": "Book Title",
  "author": "Author Name",
  "startDate": "YYYY-MM-DD",
  "image": "path/to/image.jpg"
}
```

## 4. Adding Your Data
1. Upload your JSON files to your hosting platform (e.g., GitHub).
2. Replace the `fetch` URLs in the JavaScript section with your JSON file URLs:
   ```javascript
   const readBooksURL = 'https://your-site.com/read.json';
   const wantToReadBooksURL = 'https://your-site.com/to-read.json';
   const currentlyReadingURL = 'https://your-site.com/reading.json';
   ```

## 5. Setting Up Hosting
1. **GitHub Pages**: Upload your files to a GitHub repository and enable GitHub Pages for hosting.
2. **Other Hosting Options**: Use services like Netlify, Vercel, or your preferred hosting platform.

## 6. Customize the Design
To personalize:
- Change colors, fonts, or layout by editing the CSS.
- Modify the HTML structure if needed.

## 7. Using the Website
- Add, update, or remove books by editing the JSON files.
- Use the search bar and filters to explore the book collection.
- Display the currently reading book in the dedicated section.

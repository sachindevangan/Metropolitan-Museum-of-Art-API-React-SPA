
---

# Metropolitan Museum of Art API React SPA

## Description
This project is a React Single Page Application (SPA) that utilizes the Metropolitan Museum of Art API to display information about various art objects in the museum's collection. The application uses React Router for navigation and Axios for API calls to fetch and display data. The UI is enhanced with Material-UI components, and the application follows async/await practices to optimize data fetching and handling.

## Features
- **Homepage**: Describes the application’s purpose, introduces the Metropolitan Museum of Art API, and links to the Collection page.
- **Collection Page**: Displays a paginated list of art objects. Users can navigate pages, view object images, titles, artist names, and dates, and click for detailed views.
- **Object Details Page**: Provides in-depth information about a single art object, including image, title, artist details, date, department, medium, classification, and other available metadata.
- **Pagination**: Pagination buttons allow users to navigate through the collection in a user-friendly manner, with page numbers calculated based on API data.
- **Error Handling**: Redirects to 400 and 404 pages for invalid or missing resources.
- **Extra Credit**: Optionally, users can search for art objects by keyword, with paginated search results if the search yields many matches.

## Tech Stack
- React
- Vite
- React Router 6
- Axios
- Material-UI

## API Endpoints
1. **Objects**: Returns all valid object IDs.
   - Endpoint: `https://collectionapi.metmuseum.org/public/collection/v1/objects`
2. **Object**: Fetches full details for a single object by ID.
   - Endpoint: `https://collectionapi.metmuseum.org/public/collection/v1/objects/{ObjectId}`
3. **Search**: Returns object IDs matching a query (used for optional search feature).
   - Endpoint: `https://collectionapi.metmuseum.org/public/collection/v1/search?q={query}`

## Routes
- **`/`**: Homepage with a link to the Collection page.
- **`/collection/page/:page`**: Collection page that fetches and displays a paginated list of art objects.
- **`/collection/:id`**: Object details page that displays detailed information for a specific art object.

## Installation
1. Clone the repository.
   ```bash
   git clone https://github.com/sachindevangan/Metropolitan-Museum-of-Art-API-React-SPA
   ```
2. Navigate to the project directory.
   ```bash
   cd met-museum-spa
   ```
3. Install dependencies.
   ```bash
   npm install
   ```
4. Start the development server.
   ```bash
   npm run dev
   ```

## Usage
- Access the collection and object details through the navigation links.
- (Optional) Use search to find art objects by keyword.

## License
This project is licensed under the MIT License.
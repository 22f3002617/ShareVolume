# C.H. Robinson Share Data Viewer

## Description
This web application fetches and displays the maximum and minimum number of common stock shares outstanding for C.H. Robinson (or any company specified through a CIK query parameter) from the SEC's XBRL API.

## Features
- Dynamic fetching of share data from the SEC API for specified CIK.
- Displays the maximum and minimum shares outstanding, and their respective fiscal years, for periods post-2020.
- Supports URL parameters to display data for other companies.
  
## Usage
1. Open `index.html` in a web browser.
2. Use the `?CIK=YOUR_CIK_HERE` query parameter to fetch data for a different company.

## Local Development
1. Clone the repository: `git clone REPO_URL`
2. Navigate to the project directory: `cd project-directory`
3. Open `index.html` in your web browser.

## GitHub Pages Deployment
Ensure GitHub Pages is set to serve from the main branch or a designated docs folder with `index.html` included.

## Accessibility and Fallback
- Simple, semantic HTML ensures screen-reader accessibility.
- If data cannot be fetched, the interface will display empty fields.

## Future Improvements
- Add error handling for fetch failure.
- Cache data to reduce API calls.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Assumptions
- Data is fetched from the SEC using any proxy if needed.
- Ties in max/min values can be arbitrarily broken.
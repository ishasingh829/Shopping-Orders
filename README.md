# Online Food Delivery Order Manager

A simple, web-based application to manage food delivery orders. Users can add orders, view them in a table, filter by status and distance, and automatically assign deliveries to the nearest unpaid order within a specified distance. Built with vanilla HTML, CSS, and JavaScript for easy deployment.

## Features

- **Add Order**: Input form to create new orders with restaurant name, item count, payment status, and delivery distance.
- **View All Orders**: Table displaying all orders with sorting by columns (e.g., distance, status).
- **Filter Orders**: Filter by paid/unpaid status and maximum delivery distance (≤ X KM).
- **Assign Delivery**: Automatically assigns the nearest unpaid order within a given max distance. If no order qualifies, displays "No order available."
- **Data Persistence**: Orders are saved in browser local storage, so they persist across sessions.
- **Responsive UI**: Works on desktop and mobile devices.

## Data Model

Each order includes:
- `orderId`: Unique auto-generated ID.
- `restaurantName`: Name of the restaurant.
- `itemCount`: Number of items in the order.
- `isPaid`: Boolean (true for paid, false for unpaid).
- `deliveryDistance`: Distance in KM.
- `isAssigned`: Boolean (tracks if delivery is assigned).

## Installation and Setup

1. **Download the Files**: Save `index.html` (and optionally `README.md`) to your computer.
2. **No Dependencies**: This is a static HTML file—no server or installations needed.
3. **Run Locally**: Double-click `index.html` to open in any modern web browser (e.g., Chrome, Firefox).

## Usage

1. **Add an Order**:
   - Fill the form with details (e.g., Restaurant: "Pizza Place", Item Count: 2, Status: Unpaid, Distance: 5 KM).
   - Click "Add Order". The order will appear in the table.

2. **View and Filter Orders**:
   - Scroll to the "View All Orders" section.
   - Use the filters: Select status (Paid/Unpaid) and enter max distance, then click "Apply Filters".
   - Click table headers to sort (e.g., by distance).

3. **Assign Delivery**:
   - Enter a max distance (e.g., 10 KM) in the "Assign Delivery" section.
   - Click "Assign Delivery". It will assign the nearest unpaid order or show "No order available".

4. **Testing Tips**:
   - Add multiple orders to test filtering and assignment.
   - Refresh the page—data should remain due to local storage.

## Deployment

To make the app live online:
- **Netlify (Recommended)**: Sign up at [netlify.com](https://netlify.com), click "Add new site" > "Deploy manually", upload `index.html`, and deploy. Get a free URL like `https://your-app.netlify.app`.
- **GitHub Pages**: Upload files to a GitHub repo, go to Settings > Pages, select the main branch, and enable. URL: `https://username.github.io/repo-name/`.
- **Other Options**: Vercel or Heroku for more features.

## Technologies Used

- **HTML**: Structure and forms.
- **CSS**: Styling for a clean, responsive UI.
- **JavaScript**: Logic for adding, filtering, sorting, and assigning orders. Uses local storage for data.

## Contributing

Feel free to fork this project and add features like user authentication, a backend database, or real-time updates. Submit a pull request with changes!

## License

This project is open-source under the MIT License. Use it freely for learning or assignments.
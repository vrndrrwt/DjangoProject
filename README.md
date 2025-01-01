# Food Ordering App

A feature-rich Food Ordering App built using the Django framework. This app enables users to browse menus, place orders, and track their order status while providing restaurant owners an easy way to manage their offerings and process orders.

## Features

### User Features:
- **User Authentication:** Sign up, log in, and log out functionality.
- **Menu Browsing:** Browse food items categorized by cuisine or type.
- **Order Placement:** Add items to the cart and place an order.
- **Order History:** View past orders with detailed information.
- **Order Tracking:** Real-time order status updates.

### Admin/Restaurant Owner Features:
- **Menu Management:** Add, edit, or delete food items.
- **Order Management:** View, accept, or reject orders.
- **Dashboard:** View analytics and reports.

## Tech Stack

- **Frontend:** HTML, CSS, JavaScript, Bootstrap
- **Backend:** Django Framework
- **Database:** SQLite (default, can be replaced with PostgreSQL or MySQL)
- **APIs:** Django REST Framework (for API endpoints)

## Installation

### Prerequisites:
- Python 3.9+
- pip (Python package installer)
- Virtualenv (recommended)

### Steps to Run Locally:

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/your-username/food-ordering-app.git
   cd food-ordering-app
   ```

2. **Create and Activate a Virtual Environment:**
   ```bash
   python -m venv env
   source env/bin/activate  # On Windows: env\Scripts\activate
   ```

3. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Apply Migrations:**
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

5. **Create a Superuser:**
   ```bash
   python manage.py createsuperuser
   ```

6. **Run the Server:**
   ```bash
   python manage.py runserver
   ```

7. **Access the Application:**
   Open your browser and go to `http://127.0.0.1:8000/`.

## Folder Structure

```
food-ordering-app/
├── app_name/           # Main application folder
│   ├── migrations/     # Database migrations
│   ├── static/         # Static files (CSS, JS, images)
│   ├── templates/      # HTML templates
│   ├── views.py        # View logic
│   ├── models.py       # Database models
│   ├── urls.py         # Application URLs
├── food_ordering_app/  # Project settings
├── db.sqlite3          # Default database
├── manage.py           # Django management script
├── requirements.txt    # Python dependencies
```

## API Endpoints

### User Endpoints:
- `POST /api/register/`: User registration
- `POST /api/login/`: User login
- `GET /api/menu/`: Get list of food items
- `POST /api/order/`: Place an order
- `GET /api/orders/`: View order history

### Admin Endpoints:
- `POST /api/menu/add/`: Add a new food item
- `PUT /api/menu/<id>/edit/`: Edit a food item
- `DELETE /api/menu/<id>/delete/`: Delete a food item
- `GET /api/orders/pending/`: View pending orders
- `PUT /api/orders/<id>/update/`: Update order status

## Future Improvements

- Integration with payment gateways
- Real-time notifications using WebSockets
- Mobile app version

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Contributions

Contributions are welcome! Please fork the repository and submit a pull request.

## Contact

For queries or feedback, reach out to:
- **Name:** Virendra Singh Rawat
- **Email:** virendrasinghrawat2812@gmail.com
- **GitHub:** [vrndrrwt](https://github.com/vrndrrwt)

---

Enjoy using the Food Ordering App!

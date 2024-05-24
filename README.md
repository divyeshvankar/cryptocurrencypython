```markdown
# Cryptocurrency Project

This project is a web application for a cryptocurrency platform built using Flask. It allows users to register, login, view their balance, and perform transactions. Additionally, users can buy the platform's cryptocurrency using Razorpay for payment processing.

## Features

- User registration and login
- User session management
- Transaction functionality
- Purchase cryptocurrency via Razorpay
- Blockchain implementation to handle transactions

## Installation

### Prerequisites

- Python 3.x
- MySQL server
- pip (Python package installer)

### Clone the Repository

```bash
git clone https://github.com/divyeshvankar/cryptocurrencypython.git
cd cryptocurrency-project
```

### Create and Activate a Virtual Environment

```bash
python -m venv venv
source venv/bin/activate   # On Windows use `venv\Scripts\activate`
```

### Install the Dependencies

```bash
pip install -r requirements.txt
```

### Configure MySQL

Create a MySQL database and update the `config.py` file with your Razorpay credentials.

```python
# config.py
RAZORPAY_KEY_ID = 'your_razorpay_key_id'
RAZORPAY_KEY_SECRET = 'your_razorpay_key_secret'
```

### Run the Application

```bash
python app.py
```

The application will be available at `http://127.0.0.1:5000/`.

## Project Structure

```
cryptocurrency-project/
│
├── app.py                 # Main application file
├── config.py              # Configuration file for Flask and MySQL
├── forms.py               # Form classes for handling user inputs
├── sqlhelpers.py          # Helper functions for database operations
├── templates/             # HTML templates for the web pages
│   ├── index.html
│   ├── register.html
│   ├── login.html
│   ├── dashboard.html
│   ├── transaction.html
│   ├── buy.html
│   ├── razorpay_checkout.html
│   └── ...
├── static/                # Static files (CSS, JS, images)
│   └── ...
├── blockchain.py          # Blockchain implementation
├── requirements.txt       # List of dependencies
└── README.md              # Project documentation
```

## Usage

### Register

Navigate to `/register` to create a new user account. Provide your name, email, username, and password.

### Login

Navigate to `/login` to log into your account using your username and password.

### Dashboard

After logging in, you will be redirected to the dashboard (`/dashboard`), where you can view your balance and the current blockchain status.

### Transactions

Navigate to `/transaction` to send money to another user. Provide the recipient's username and the amount to send.

### Buy Cryptocurrency

Navigate to `/buy` to purchase cryptocurrency using Razorpay. Enter the amount you wish to buy and proceed with the payment. Upon successful payment, the purchased cryptocurrency will be credited to your account.

## Blockchain

The project includes a basic blockchain implementation. Each transaction is added as a block in the blockchain. The blockchain ensures data integrity and security.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

- Flask framework: [Flask](https://flask.palletsprojects.com/)
- Razorpay: [Razorpay](https://razorpay.com/)
- Passlib for password hashing: [Passlib](https://passlib.readthedocs.io/)
- MySQL database: [MySQL](https://www.mysql.com/)

## Contact

For any questions or suggestions, feel free to contact me at [divyeshvankar.iitg@gmail.com].


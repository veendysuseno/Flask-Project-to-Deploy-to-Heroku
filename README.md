# Flask Project - Deploy to Heroku

This repository contains a basic Flask web application that is configured to be deployed on Heroku. Follow the instructions below to set up, run, and deploy the project to Heroku.

## Prerequisites

Before you start, make sure you have the following tools installed:

- [Python 3.x](https://www.python.org/downloads/)
- [Git](https://git-scm.com/)
- [Heroku CLI](https://devcenter.heroku.com/articles/heroku-cli)

## Setup

1. **Clone the Repository**

   Clone this repository to your local machine:

   ```bash
   git clone https://github.com/your-username/flask-project-to-heroku.git
   ```

2. Navigate to the Project Directory

   ```bash
   cd flask-project-to-heroku
   ```

3. Create and Activate a Virtual Environment

- Create a virtual environment to manage project dependencies:

```bash
python -m venv Flask-Project
```

Activate the virtual environment: <br/>

- On Windows:

```bash
venv\Scripts\activate
```

- On macOS/Linux:

```bash
source venv/bin/activate
```

4. Install Dependencies

- Install the required Python packages:

```bash
pip install -r requirements.txt
```

5. Configure Environment Variables

Create a .env file in the root directory of your project and add any required environment variables. For example:

```plaintext
FLASK_APP=app.py
FLASK_ENV=development
```

## Running Locally

To run the Flask application locally, use the following command:

```bash
flask run
```

- Visit http://127.0.0.1:5000 in your browser to see the application in action.

## Deployment to Heroku

1. Login to Heroku
   - Log in your Heroku account using the Heroku CLI:
   ```bash
   heroku login
   ```
2. Create a Heroku Application
   - Create a new Heroku application:
   ```bash
   heroku create your-app-name
   ```
3. Add a Heroku Remote
   - Add a Heroku remote your local Git repository:
   ```bash
   heroku git:remote -a your-app-name
   ```
4. Deploy to Heroku
   - Deploy the application to Heroku:
   ```bash
   git add .
   git commit -m "Initial commit"
   git push heroku master
   ```
5. Open the Application
   - Open your deployed application in the browser:
   ```bash
   heroku open
   ```

## Heroku Configuration

Make sure you have the following files in your project for Heroku deployment:

- Procfile: Specifies the commands to run the application.
  ```bash
  web: gunicorn app:app
  ```
- requirements.txt: Lists the Python dependencies.
- runtime.txt: Specifies the Python version (e.g., python-3.8.10).

## License

This project is open-source and available under the MIT License.

For more information on deploying Flask applications to Heroku, refer to the Heroku Documentation.

### Penjelasan Struktur `README.md`:

1. **Prerequisites**: Menyebutkan alat yang diperlukan sebelum memulai.
2. **Setup**: Langkah-langkah untuk menyiapkan proyek secara lokal, termasuk cloning repositori, membuat dan mengaktifkan lingkungan virtual, serta menginstal dependensi.
3. **Running Locally**: Instruksi untuk menjalankan aplikasi Flask di lingkungan lokal.
4. **Deployment to Heroku**: Langkah-langkah untuk meng-deploy aplikasi ke Heroku, termasuk login, membuat aplikasi, menambahkan remote, dan melakukan deployment.
5. **Heroku Configuration**: Daftar file penting yang diperlukan untuk Heroku deployment.
6. **License**: Menyebutkan lisensi proyek dan tautan ke dokumentasi Heroku untuk informasi lebih lanjut.

README ini memberikan panduan lengkap tentang bagaimana mengatur dan meng-deploy proyek Flask ke Heroku.
<br/>
"# Flask-Project-to-Deploy-to-Heroku" 

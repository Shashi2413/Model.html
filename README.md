Smart Register Flask App 

This is a simple inventory management and financial tracking applicaƟon built with Flask, 

HTML, Tailwind CSS, and JavaScript. It allows users to add new items to inventory, view 

exisƟng inventory, and modify stock quanƟƟes due to sales or damage, while also tracking 

profit and loss. 

Features 

 Add New Items: Easily add items with unique IDs, names, quanƟƟes, and cost prices.
 Inventory & ValuaƟon View: See a comprehensive list of all inventory items, 

including total unique items, total quanƟty, and total inventory value.

 Search FuncƟonality: Quickly find items in the inventory using a search bar. 

 Stock ModificaƟon: Adjust item quanƟƟes for sales or damage, with automaƟc 

calculaƟon of profit or loss.

 Financial Summary: View a real-Ɵme summary of total profit and total loss.

 Local Storage Persistence: All inventory and financial data are saved locally in the 

browser, persisƟng across sessions.

 Responsive Design: The applicaƟon is designed to be usable on various screen sizes 

(mobile, tablet, desktop). 

Project Structure 

The project follows a standard Flask applicaƟon structure:

. 

├── app.py 

├── requirements.txt 

├── Procfile 

├── templates/ 

│ └── index.html 

└── staƟc/

 ├── styles.css 

 └── script.js 

 app.py: The main Flask applicaƟon file, handling routes and rendering templates.

 requirements.txt: Lists Python dependencies for the project. 

 Procfile: Specifies the command to run the applicaƟon on plaƞorms like Render.

 templates/: Contains HTML template files (e.g., index.html). 

 staƟc/: Contains staƟc assets like CSS (styles.css) and JavaScript (script.js). 

Technologies Used 

 Flask: Python web framework.
 HTML5: Structure of the web pages. 

 Tailwind CSS: UƟlity-first CSS framework for styling. 

 JavaScript: Client-side logic for interacƟve features and data persistence (using Local 

Storage). 

 Gunicorn: WSGI HTTP Server for producƟon deployment.

Setup and InstallaƟon

Follow these steps to get the Smart Register app up and running on your local machine. 

Prerequisites 

 Python 3.x installed on your system. 

Steps 

1. Clone the repository:

2. git clone hƩps://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git

3. cd YOUR_REPOSITORY_NAME 

4. Create a virtual environment (recommended):

5. python -m venv venv 

6. AcƟvate the virtual environment:

o On macOS/Linux:

o source venv/bin/acƟvate

o On Windows:

o venv\Scripts\acƟvate

7. Install the dependencies:

8. pip install -r requirements.txt 

9. Run the Flask applicaƟon:

10. python app.py 

The applicaƟon will typically run on hƩp://127.0.0.1:5000/. Open this URL in your web 

browser. 

Deployment on Render 

This applicaƟon is configured for easy deployment on Render.com.

1. Push your code to a GitHub repository.

2. Create a new Web Service on Render.

3. Connect your GitHub repository.

4. Configure the build and start commands:

o Build Command: pip install -r requirements.txt 

o Start Command: gunicorn app:app 

5. Deploy! Render will automaƟcally detect your Procfile and requirements.txt to build 

and run your applicaƟon.

Usage 

 Navigate between "Add Item", "Inventory & ValuaƟon", and "Stock ModificaƟon" 

screens using the navigaƟon buƩons.

 On the "Add Item" screen, fill in the details and click "Add Item" to add new 

inventory. 

 On the "Inventory & ValuaƟon" screen, you can view your current stock and search 

for items. 

 On the "Stock ModificaƟon" screen, select an item, enter the quanƟty to change, 

choose the reason (Sale or Damage), and apply the change. If it's a sale, specify the 

sale price.


10. Conclusion 

The Smart Register Flask App provides a funcƟonal and intuiƟve soluƟon for basic inventory 

and financial tracking. By leveraging modern web technologies and simple data persistence, 

it offers a quick and easy way for users to manage their stock. Its modular design and clear 

separaƟon of concerns (Flask for backend, dedicated files for HTML, CSS, and JS) make it 

maintainable and extensible. While currently relying on client-side storage, the architecture 

allows for straighƞorward future enhancements to integrate a database and expand its 

capabiliƟes for more advanced business needs. This project serves as a solid foundaƟon for a 

comprehensive inventory management system.

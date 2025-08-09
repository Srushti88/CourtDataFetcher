# Delhi High Court Case Details Scraper

This is a Python Flask application that allows users to fetch case details from the Delhi High Court website using a clean and responsive web interface. The application scrapes case data based on user input, caches results in an SQLite database, and displays them with styled HTML templates. Users can also download the latest order PDFs.

---

## 🔧 Features

- ✅ Submit case type, number, and year via web form  
- ✅ Scrapes case data from the [Delhi High Court](https://delhihighcourt.nic.in/) website  
- ✅ Caches and stores results in SQLite database  
- ✅ Responsive and styled results page using Jinja2 templates  
- ✅ Graceful handling of invalid or missing case inputs  
- ✅ Built-in test cases for validation and reliability  
- ✅ Download latest order PDFs directly from the results page  

---

## 📦 Setup Instructions

```bash
git clone https://github.com/Srushti88/CourtDataFetcher.git
cd CourtDataFetcher
python3 -m venv venv
# On Linux/macOS
source venv/bin/activate
# On Windows (PowerShell)
venv\Scripts\activate
pip install -r requirements.txt


##  Run Locally
$env:FLASK_APP = "main.py"
$env:FLASK_ENV = "development"
flask run


## On Unix/Linux/macOS (bash/zsh)
export FLASK_APP=main.py
export FLASK_ENV=development
flask run


## After running the commands, open your browser and navigate to: 
http://localhost:5000


##  Run Tests
- python test_cases.py


## 📝 Project Structure
```
CourtDataFetcher/
├── main.py               
├── scraper.py           
├── models.py             
├── dto.py                
├── templates/            
│   ├── case_input_form.html  
│   └── result.html           
├── test_cases.py         
├── requirements.txt      
└── README.md             
```


## Contributing
```
Pull requests are welcome! For significant changes or feature requests, please open an issue first to discuss.
```

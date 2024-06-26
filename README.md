# E-Commerce Comparison Project
This project aims to compare product features and prices between the Trendyol and Amazon Turkey e-commerce platforms. Data is collected using web scraping techniques and stored in a MySQL database.

## Table of Contents

1. [Technologies Used](#technologies-used)
2. [Installation](#installation)
3. [Usage](#usage)
4. [Usage](#usage)
5. [Database Structure](#database-structure)
6. [Sources](#sources)

## Technologies Used

-Python 3

-BeautifulSoup

-Requests

-MySQL Connector/Python

-PyMySQL

## Installation

### 1. Clone the Repository

```bash
    git clone https://github.com/200202087/webscraping.git
    cd webscraping
```


### 2. Install Required Python Packages


### 3. Create MySQL Database and Table

```bash
    CREATE DATABASE prolan;
    USE prolan;

    CREATE TABLE tablo (
    num INT AUTO_INCREMENT PRIMARY KEY,  
    ozel VARCHAR(255),  
    ism VARCHAR(255),
    fiyat VARCHAR(50),  
    lptp_tam TEXT
);
```

### 4. Update Database Connection Settings

Update the database connection information in the main.py file to match your MySQL server:

```bash
    moba = pymysql.connect(
    user='root',
    password='1234',
    host='127.0.0.1',
    db='prolan',
    charset='utf8mb4',
    cursorclass=pymysql.cursors.DictCursor
)
```

## Usage

### 1. Collect Data

Run the following command to start the data collection process:
python main.py

### 2. Examine Data

The data will be stored in the tablo table in the MySQL database. You can use a MySQL client or a database management tool to examine the data.

Database Structure

num: Product number (auto-increment primary key)

ozel: Product features

ism: Feature name

fiyat: Product price

lptp_tam: Product URL


## Sources

You can review the project interface code [here](Arayuz.php).

You can review the project backend code [here](WebScraping.py).

You can review the project report [here](WebScrapingRep.pdf).

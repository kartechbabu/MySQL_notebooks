# MySQL notebooks

Runnable Python and R notebooks for **ITOM 6265 Database Design for Business**
(SMU). They connect to a MySQL 8 database and are written to open in
[Google Colab](https://colab.research.google.com/) as well as in Jupyter or
VS Code.

The notebooks are added here as the course book publishes them. Each one is
explained in the book: <https://itom6265-database-design.netlify.app/>.

| Notebook | Open |
|---|---|
| `csv_to_mysql_python.ipynb`: load a CSV file into MySQL with pandas | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kartechbabu/MySQL_notebooks/blob/main/csv_to_mysql_python.ipynb) |
| `csv_to_mysql_r.ipynb`: the same with readr, DBI and RMariaDB | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kartechbabu/MySQL_notebooks/blob/main/csv_to_mysql_r.ipynb) |

In Colab, use **File → Save a copy in Drive** to keep your own editable copy.

## Data

`data/` holds the sample files the notebooks read:

- `london_restaurants.csv`: 15 London restaurants from the class's Zomato data.
- `london_restaurants_update.csv`: 5 more restaurants, plus a newer row for
  Gymkhana. Its vote count, 230, is invented to demonstrate an update.

## Credentials

Never put a password in a notebook. In Colab, store `DB_HOST`, `DB_PORT`,
`DB_USER`, `DB_PASSWORD` and `DB_NAME` as **Secrets** (key icon in the left
sidebar). On your own computer, put them in a `.env` file next to the
notebook. `.env` files are ignored by this repository.

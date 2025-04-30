## 📊 Data Preparation

### 🔍 Data Examination

In the initial phase of the project, I examined the original data files provided in CSV format. Below is a summary of the structure and content of each file:

---

#### 📁 `accounts.csv` — Company Information

| Column            | Description                                           |
|-------------------|-------------------------------------------------------|
| `account`         | Company name                                          |
| `sector`          | Industry sector of the company                        |
| `year_established`| Year the company was established                      |
| `revenue`         | Annual revenue (in millions USD)                      |
| `employees`       | Number of employees                                   |
| `office_location` | Headquarters location                                 |
| `subsidiary_of`   | Parent company, if applicable                         |

---

#### 📁 `sales_teams.csv` — Sales Agent and Manager Details

| Column           | Description                          |
|------------------|--------------------------------------|
| `sales_agent`    | Name of the sales agent              |
| `manager`        | Name of the respective sales manager |
| `regional_office`| Location of the regional office      |

---

#### 📁 `products.csv` — Product Details

| Column        | Description                        |
|---------------|------------------------------------|
| `product`     | Product name                       |
| `series`      | Product series or family           |
| `sales_price` | Suggested retail price             |

---

#### 📁 `sales_pipeline.csv` — Sales Opportunity Records

| Column           | Description                                                       |
|------------------|-------------------------------------------------------------------|
| `opportunity_id` | Unique identifier for each sales opportunity                      |
| `sales_agent`    | Sales agent responsible for the opportunity                       |
| `product`        | Product involved in the opportunity                               |
| `account`        | Company involved in the opportunity (nullable)                    |
| `deal_stage`     | Stage of the sales pipeline (e.g., Prospecting > Won / Lost)      |
| `engage_date`    | Date when the deal was moved to the "Engaging" stage (nullable)   |
| `close_date`     | Date when the deal was either won or lost (nullable)              |
| `close_value`    | Revenue generated from the deal (nullable)                        |

---

Initially, the `sales_pipeline.csv` file contained full names for `sales_agent`, `product`, and `account` fields, referencing `sales_teams.csv`, `products.csv`, and `accounts.csv`. 

To optimize the data structure for performance and consistency, **ID columns** were added to these three reference files and used in the `sales_pipeline.csv` file instead.

---

## 🔄 Data Transformation

To prepare the data for efficient analysis, the following transformation steps were implemented:

1. **Add ID Columns**  
   Unique identifiers were added to `products.csv`, `accounts.csv`, and `sales_teams.csv`.

2. **Create Mapping Dictionaries**  
   Python dictionaries were created to map each ID to its original name for accurate replacement and traceability.

3. **Validate Data Consistency**  
   The mappings were cross-checked with `sales_pipeline.csv` to find and fix mismatches or missing references.

4. **Correct Misspelled Values**  
   Detected and corrected any inconsistencies or spelling errors across all related files.

5. **Replace Full Names with IDs**  
   The name-based fields in `sales_pipeline.csv` were replaced with the new numeric IDs for optimized performance.

6. **Save Updated Data**  
   All cleaned and transformed data was saved into new CSV files ready for import into the analysis environment.

---

### ⚠️ Columns with Empty Values

| File              | Columns with Empty Values                          |
|-------------------|----------------------------------------------------|
| `accounts.csv`    | `subsidiary_of`                                    |
| `sales_pipeline.csv` | `account`, `engage_date`, `close_date`, `close_value` |

---

## 🛠️ Tools & Output

- **Language**: Python  
- **Script**: Included in a Jupyter Notebook  
- **Notebook**: `csv_files_preparation.ipynb`  
- **Transformed Files Directory**: `Modified_Files/`

This automated process ensured a clean, standardized, and analysis-ready dataset for the next phases of the CRM Sales Analysis project.

---

# CSV to SQLite Importer for Soil Flux Database

This script imports data from a CSV file into an SQLite database, ensuring that duplicate columns for `plot_number` and `Date_time` are handled appropriately. Before running the main GUI application (`gui_soil.py`), this script **must be executed** to ensure the database is properly populated.

## Usage

1. **Pre-requisite:**
   - Ensure that the SQLite database file is located at `/Users/sanskarsrivastava/Desktop/CSE/Database-job/post_soil_flux.db`.   This location can be changed accordingly
   - **Important**: The location and name of the database file should **never change**. This is crucial for the seamless integration between the importer script and the `gui_soil.py` application.

2. **Steps:**
   - Run this Python script to import the CSV data into the database.
   - The script will create a table named `post_soil_flux` if it doesn't already exist.
   - Any duplicate columns for `plot_number` and `Date_time` will be skipped to avoid conflicts.

3. **Execution:**
   Run the script before launching the GUI application.

   ```bash
   python gui_soil.py
   ```

4. **CSV File Path:**
   The CSV file used for importing is located at:
   `/Users/sanskarsrivastava/Desktop/CSE/Database-job/Data/Processed_full_fluxes_Map_file_soil_QUI-02_2023-05-05.csv`.   This location can be changed accordingly

5. **Integration with GUI: This import script must be executed before running the GUI application (gui_soil.py), which depends on the data populated by this script. For more details about the project, visit the repository: Database Job on GitHub.

---


## File Content Description

### `datasets/indie-games-developers.csv`

This CSV file contains information about indie game developers, including:

*   **Developer:** Name of the indie game developer.
*   **City:** City where the developer is located.
*   **Autonomous area:** Autonomous area or region within the country (e.g., state, province).
*   **Country:** Country where the developer is located.
*   **Notable games:** A list of notable games developed by the studio.
*   **Notes:** Additional information about the developer.

### `datasets/vgsales.parquet`

This Parquet file contains video game sales data. The structure of this dataset requires pandas and pyarrow to be opened correctly. Columns include:

*   **Rank:** Overall rank of the game based on global sales.
*   **Name:** Name of the game.
*   **Platform:** Platform on which the game was released.
*   **Year:** Year of the game's release.
*   **Genre:** Genre of the game.
*   **Publisher:** Publisher of the game.
*   **NA_Sales:** North American sales (in millions).
*   **EU_Sales:** European sales (in millions).
*   **JP_Sales:** Japanese sales (in millions).
*   **Other_Sales:** Sales in other regions (in millions).
*   **Global_Sales:** Total global sales (in millions).

### `datasets/video-games-developers.csv`

This CSV file contains information about video game developers, including:

*   **Developer:** Name of the video game developer.
*   **City:** City where the developer is located.
*   **Administrative division:** Administrative division or region within the country.
*   **Country:** Country where the developer is located.
*   **Notable games, series or franchises:** A list of notable games, series, or franchises developed by the studio.
*   **Est.:** Establishment year
*   **Notes:** Additional information about the developer.

### `notebooks/datasets2.ipynb`

This Jupyter Notebook demonstrates basic data processing and cleaning using the datasets:

*   Loading and inspecting the `vgsales.parquet` dataset using Pandas.
*   Setting the 'Publisher' column as the index.
*   Dropping the 'Rank' column.
*   Handling missing values (NaN).
*   Loading and inspecting `indie-games-developers.csv` and `video-games-developers.csv`.
*   Dropping irrelevant columns from the CSV files.
*   Concatenating the indie and general developer CSV files.
*   Removing duplicate developer entries based on the 'Developer' column.
*   Performing initial data exploration and cleaning.

## Usage

1.  Clone this repository to your local machine.
2.  (Optional) Create a virtual environment for the project:
    ```bash
    python3 -m venv venv
    source venv/bin/activate  # On Linux/macOS
    venv\Scripts\activate  # On Windows
    ```
3.  Install the required libraries:
    ```bash
    pip install pandas pyarrow jupyter
    ```
4.  Open the `notebooks/datasets2.ipynb` notebook using Jupyter Notebook or JupyterLab:
    ```bash
    jupyter notebook notebooks/datasets2.ipynb
    ```
    or
    ```bash
    jupyter lab notebooks/datasets2.ipynb
    ```
5.  Run the cells in the notebook to explore and process the data.

## Potential Future Work

*   Implement data visualization techniques in the notebook to gain insights from the datasets.
*   Develop more advanced data cleaning and transformation steps.
*   Explore the relationships between game sales, genres, publishers, and developers.
*   Add more datasets related to video games, such as game reviews or player statistics.
*   Populate the `main.py` file with scripts for automated data processing or analysis.

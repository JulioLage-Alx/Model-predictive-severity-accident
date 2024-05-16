# Data Analysis and Prediction Model Project

Welcome to the Data Analysis and Prediction Model Project! This repository contains all the code, data, and documentation needed to understand, execute, and expand the analyses and predictions performed.

## Table of Contents

- [Description](#description)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Data](#data)
- [Models](#models)
- [Contribution](#contribution)
- [License](#license)
- [Data Dictionary](#data-dictionary)

## Description

This project was developed to analyze a specific dataset and build a predictive model based on that data. The goal is to provide useful insights and predictions that can aid in decision-making.

## Project Structure

The project directory structure is as follows:

```
.
├── data
│   ├── raw                # Raw, unprocessed data
│   ├── processed          # Processed data ready for analysis
├── notebooks              # Jupyter notebooks for exploratory analysis
├── scripts
│   ├── data_processing.py # Script for data processing
│   ├── model_training.py  # Script for model training
│   ├── model_evaluation.py# Script for model evaluation
├── models                 # Trained models and their versions
├── results                # Analysis and prediction results
├── requirements.txt       # Project dependencies
└── README.md              # Project documentation
```

## Installation

To install and run this project locally, follow the steps below:

1. Clone the repository:
   ```bash
   git clone https://github.com/JulioLage-Alx/Model-predictive-severity-accident
   ```

2. Navigate to the project directory:
   ```bash
   cd Model-predictive-severity-accident
   ```

3. Create a virtual environment:
   ```bash
   python -m venv venv
   ```

4. Activate the virtual environment:
   - On Windows:
     ```bash
     venv\Scripts\activate
     ```
   - On Unix or MacOS:
     ```bash
     source venv/bin/activate
     ```

5. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

### Data Processing

To process the raw data, use the `data_processing.py` script:

```bash
python scripts/data_processing.py
```

### Model Training

To train the model, use the `model_training.py` script:

```bash
python scripts/model_training.py
```

### Model Evaluation

To evaluate the model's performance, use the `model_evaluation.py` script:

```bash
python scripts/model_evaluation.py
```

### Jupyter Notebooks

You can also explore the data and perform analyses in the Jupyter notebooks available in the `notebooks` folder. To start the Jupyter Notebook, use:

```bash
jupyter notebook
```

## Data

The data used in this project is located in the `data` folder. Raw data should be placed in the `raw` folder, while processed data will be in the `processed` folder after running the processing scripts.

## Models

Trained models are saved in the `models` folder. Each model is versioned and stored for future comparisons and improvements.

## Contribution

Contributions are welcome! If you wish to contribute to this project, please follow the steps below:

1. Fork this repository.
2. Create a branch for your feature or bug fix (`git checkout -b feature/new-feature`).
3. Commit your changes (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature/new-feature`).
5. Open a Pull Request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---

We hope this project is useful and that you can learn and contribute to it. If you have any questions, feel free to open an issue or contact us.

Happy analyzing and predicting!

# Data Dictionary

## Description:
This comprehensive dataset provides detailed information on road accidents reported over several years. The dataset encompasses various attributes related to accident status, vehicle and casualty references, demographics, and casualty severity. It includes essential factors such as pedestrian details, casualty types, road maintenance worker involvement, and the Index of Multiple Deprivation (IMD) decile for the casualties' residential areas.

## Columns:

- **Status**: The status of the accident (e.g., reported, under investigation)
- **Accident_Index**: A unique identifier for each reported accident
- **Accident_Year**: The year the accident occurred
- **Accident_Reference**: A reference number associated with the accident
- **Vehicle_Reference**: A reference number for the vehicle involved in the accident
- **Casualty_Reference**: A reference number for the casualty involved in the accident
- **Casualty_Class**: Indicates the class of the casualty (e.g., driver, passenger, pedestrian)
- **Sex_of_Casualty**: The sex of the casualty (male or female)
- **Age_of_Casualty**: The age of the casualty
- **Age_Band_of_Casualty**: The age band to which the casualty belongs (e.g., 0-5, 6-10, 11-15)
- **Casualty_Severity**: The severity of the casualty's injuries (e.g., fatal, serious, slight)
- **Pedestrian_Location**: The location of the pedestrian at the time of the accident
- **Pedestrian_Movement**: The movement of the pedestrian during the accident
- **Car_Passenger**: Indicates if the casualty was a car passenger at the time of the accident (yes or no)
- **Bus_or_Coach_Passenger**: Indicates if the casualty was a bus or coach passenger (yes or no)
- **Pedestrian_Road_Maintenance_Worker**: Indicates if the casualty was a road maintenance worker (yes or no)
- **Casualty_Type**: The type of casualty (e.g., driver/rider, passenger, pedestrian)
- **Casualty_Home_Area_Type**: The type of area where the casualty resides (e.g., urban, rural)
- **Casualty_IMD_Decile**: The IMD decile of the area where the casualty resides (a measure of deprivation)
- **LSOA_of_Casualty**: The Lower Super Output Area (LSOA) associated with the casualty's location

> [!NOTE]
> This dataset provides valuable information for analyzing road accidents, identifying trends, and implementing safety measures to reduce casualties and improve road safety. Researchers, policymakers, and analysts can leverage this dataset for evidence-based decision-making and enhance overall road transport systems.
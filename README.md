# **Multilanguage Data Generation**

## 📗 ***Table of Contents***

1. [📖 About the Project](#-about-the-project)
2. [Tech Stack](#tech-stack)
3. [💻 Getting Started](#getting-started)
   - [Installation](#installation)
   - [Dependencies](#dependencies)
   - [Usage](#usage)
     - [Generating Language-Specific JSONL Files](#generating-language-specific-jsonl-files)
     - [Consolidating Translations to JSON](#consolidating-translations-to-json)
   - [Configuration](#configuration)
4. [👥 Authors](#-authors)
5. [🤝 Contributing](#-contributing)
6. [📝 License](#-license)


## 📖 **About the Project**

Set up a Python3 development environment, import a dataset, generate en-xx.xlsx files, jsonl files for multiple languages, and create a consolidated JSON file for translations from English to other languages. This project aims to handle multilanguage data generation effectively.

### **Tech Stack**

- Python
- Visual Studio Code IDE

## 💻 **Getting Started**

To get a local copy up and running, follow these steps.

### **Installation**

1. Clone this repository to your desired folder using the following command:

      ```shell
      cd Group_CAT 
      git clone https://github.com/George-Stephen/Group_CAT

2. Set up your Python3 development environment using the following command:

   ```shell
   python -m venv env

3. Activate your Python3 development environment using the following command:

   ```shell
   env\Scripts\activate

4. Install all relevant dependencies using the following commands:

   ```shell
   pip install -r requirements.txt

### **Dependencies**

Ensure you have the following dependencies installed:
- Download Python 3.x : Click on the following link to download Python https://www.python.org/
- Download an IDE environment that well suites you i.e PyCharm https://www.jetbrains.com/help/pycharm/installation-guide.html#silent
- Setup an environment using either pip or you can use Anaconda, which will automatically create an environment for you. Click the following link to download Anaconda https://www.anaconda.com/download
- Make sure to set the Python interpreter as the environment you will be using for this project
- Pandas: You can install it using pip with
   ```shell
   pip install pandas
  
- openpyxl: Used to read and write Excel files. You can install it using the command
   ```shell
   pip install openpyxl

### **Usage**

This project provides a set of tools and scripts to generate language-specific JSONL files and consolidate translations from English to other languages in a formatted JSON file.

*Generating Language-Specific JSONL Files*

To generate language specific JSONL files for English (en), Swahili (sw), and German (de) in test, train, and dev sets, follow these steps:

1. Ensure you have Python installed on your system.
2. Clone this repository to your desired folder:
   ```shell
   git clone https://github.com/George-Stephen/Group_CAT
   cd Group_CAT

3. Navigate to the data folder and place your input data files in the corresponding language directories (e.g., en, sw, de) inside the data folder.
4. Open a terminal or command prompt and navigate to the project's root directory.

5. Run the following command to generate the JSONL files for each language:
   ```shell
   python generate_jsonl.py

**Consolidating Translations to JSON**
To consolidate translations from English to other languages into a formatted JSON file, follow these steps:

1. After generating the language-specific JSONL files, ensure they are available in the output directories.
2. Run the following command to consolidate translations:
   ```shell
   python consolidate_translations.py

3. The consolidated JSON file, named translations.json, will be created in the project's root directory.
   ```shell
   python consolidate_translations.py

### **Configuration**

To configure the project for your specific environment, you may need to make the following changes:

1. **Import and Extract the Amazon massive data file**: Declare the file path and use the tarfile library to extract content from the **Amazon Massive Data file** into an already created directory.

2. **Data Directory**: Update the `data_directory` variable in the code to point to the directory containing your JSONL files.
   
   python
   data_directory = r'path/to/your/data_directory'
   

3. **Output Directory**: Update the `output_dir` variable to specify where you want to save the generated Excel files.
   
   python
   output_dir = r'path/to/your/output_directory'
   

4. **Keyword and Field**: When running the script, you can specify the keyword and field for filtering using the `--keyword` and `--field` arguments.
   
   shell
   python script_name.py --keyword your_keyword --field your_field


## 👥 **Authors**

👤 Jackson Lowasa
      GitHub: @githubhandle

👤 George Steven
      GitHub: @githubhandle
      
👤 Charity Claire
      GitHub: @githubhandle

👤 Shaleen Ndirangu
      GitHub: @githubhandle

👤 Mwangi Patience
      GitHub: @githubhandle


## 🤝 **Contributing**

Contributions, issues, and feature requests are welcome!


## 📝 **License**

This project is licensed under the MIT License
 
 

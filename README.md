# Bug-Detection-Fixing
This project uses Machine Learning to automatically identify bugs in code and suggest fixes using the Gemini API.

Project Structure
data/: Contains training and testing datasets
models/: Saved model checkpoints
src/: Source code for the project
data_preparation.py: Scripts to collect and prepare code data
model.py: ML model architecture for bug detection
train.py: Model training code
evaluate.py: Evaluation scripts and metrics calculation
gemini_api.py: Gemini API integration for fix recommendations
utils.py: Helper functions
main.py: Entry point for the application
config.py: Configuration settings
requirements.txt: Required dependencies(compatible with python 3.11 64-bit)
Setup
Clone this repository
Install the dependencies:
pip install -r requirements.txt
Set up your environment variables:
# Create a .env file with your Gemini API key
GEMINI_API_KEY=your_api_key_here
Usage
Run this main script(preferably) to analyze all the code samples loaded in the 'samples' folder at a time:

python main.py
Run this main script to analyze all the code samples loaded in the 'samples' folder:

python main.py --analyze-file "path to that code sample"
Features
Automatic bug detection using ML models
Bug classification by type
Fix recommendations using Gemini API
Performance metrics for model evaluation

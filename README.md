# LLM Classification
This project classifies GitHub issues by domains and subdomains using a fine-tuned GPT model. 
The script processes data from an SQLite database, prepares training data, fine-tunes a GPT model, and then classifies open issues in a specified GitHub repository.

## Installation
Refer to the requirements.txt file and ensure that each library is installed as well as the appropriate version

## Use
To run, change the working directory to the location of the python script and run the following command:
python your_script.py --config path/to/conf.json --domains path/to/Domains.json --db path/to/main.db

Example:
python your_script.py --config config/conf.json --domains config/Domains.json --db data/main.db

## Conf File
The configuration json includes data necessary to run such as the desired repo or access tokens. Example:
{
    "github_token": "your_github_token",
    "repo_owner": "repository_owner",
    "repo_name": "repository_name",
    "openAI_key": "your_openai_api_key"
}

## Domains
The Domains json file includes domains, subdomains, and descriptions. This should be downloaded from the repo to ensure you work with a good set of domains.

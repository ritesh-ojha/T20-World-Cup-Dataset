# T20 World Cup Dataset README

## Introduction

Welcome to the T20 World Cup Dataset! This project is designed to manage and store data related to the T20 Cricket World Cup, including teams, players, matches, and statistics. This README provides an overview of the project, usage guidelines, and contribution protocols.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Usage](#usage)
- [Structure](#introduction)
- [Data Schema](#data-schema)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Features
- Team Management: Add, update, and delete teams participating in the T20 World Cup.

- Player Management: Add, update, and delete player information.

- Match Records: Store and retrieve match details including scores, dates, and venues.

- Statistics: Generate and view various statistics related to players and teams.

- Search Functionality: Efficiently search for teams, players, and match details.

- Data Export/Import: Export and import data in CSV format for easy sharing and backup.

## Usage

- The `code/Base package.zip` file contains all the scraping scripts and raw files used to generate this dataset.

- You can extract and run these scripts if you wish to recreate the dataset from scratch or modify the scraping logic for future updates.


## Structure
```
t20-world-cup-dataset/
├── code/
        ├── Base package.zip    # Contains all scraping scripts and raw files
├── README.md                   # This README file
├── data/                       # Data storage directory
        ├── csv/
        ├── json/
        ├── zip/                 
├── models/                     # Data models


```
## Data Schema

- ### Season
    ```json
    {
        "season_id": "integer",
        "name": "string",
        "year": "string",
        "description": "string",
        "season": "string",
        "startDate": "string",
        "endDate": "string",
        "totalSquads": "integer"
    }
    ```
- ###  Teams
    ```json
    {
        "team_id": "integer",
        "team_name": "string",
        "team_abbrevaion": "string",
        "image": "string",
        "country_id": "integer"
    }   
    ```
- ### Matches
    ```json
    {
        "season_id": "integer",
        "match_id": "integer",
        "slug": "string",
        "title": "string",
        "time_of_day": "string",
        "date": "string",
        "time": "string",
        "status": "string",
        "status_description": "string",
        "winner_team_id": "integer",
        "toss_winner_team_id": "integer",
        "toss_choice": "integer",
        "ground_id": "integer",
        "team_1_id": "integer",
        "team_2_id": "integer",
        "team_1_score": "string",
        "team_1_scoreInfo": "string",
        "team_2_scoreInfo": "string"
    }   
    ```
- ### Grounds
    ```json
    {
        "Ground ID": "integer",
        "Ground Name": "string",
        "Ground Slug": "string",
        "Town ID": "integer",
        "Capacity": "string"
    }
    ```
- ### Ball By Balls
    ```json
    {
    "index": "integer",
    "match_id": "integer",
    "inningNumber": "integer",
    "overNumber": "integer",
    "ballNumber": "integer",
    "oversUnique": "integer",
    "oversActual": "integer",
    "batsmanPlayerId": "integer",
    "bowlerPlayerId": "integer",
    "pitchLine": "string",
    "pitchLength":"string",
    "isFour": "string",
    "isSix": "string",
    "isWicket": "string",
    "byes": "integer",
    "legbyes": "integer",
    "wides": "integer",
    "noballs": "integer",
    "penalties": "integer",
    "run": "integer",
    "batsmanRuns": "integer",
    "totalRuns": "integer",
    "totalWickets": "integer",
    "outPlayerId": "integer",
    "shotType": "string"
    }

    ```
- ### Countrys
    ```json
    {
        "Country ID": "integer",
        "Country Name": "string",
        "Country Abbreviation": "string"
    }
    ```
- ### Towns
    ```json
    {
        "Town ID": "integer",
        "Town Name": "string",
        "Country ID": "integer"
    }
    ```

## Contributing
We welcome contributions! Please follow these steps:
1. Fork the repository

2. Create a new branch
    ```sh
    git checkout -b feature/your-feature-name
    ```
3. Commit your changes
    ```sh
    git commit -m "Add your message here"
    ```

4. Push to the branch
    ```sh
    git push origin feature/your-feature-name
    ```
5. Open a Pull Request

## License

This project is licensed under the Apache License. See the `LICENSE` file for more details.


## Contact

For any questions or suggestions, please contact:

- Name: Ritesh Ojha
- Email: riteshojha2002@gmail.com
- GitHub: [ritesh-ojha](https://github.com/ritesh-ojha)

Thank you for using the T20 World Cup Warehouse!


# NER-musicbrainz
 
# Named entity recognition using MUSICBRAINZ API

Problem:
- Music personalities not identified in other databases

Main notebook:
- NER.ipynb

Approach
- Use MusicBrainz database and its API to search for entities missing
- Use musicbrainzngs python library to use the API
- Retrieve list of candidate names
- Use cosine similarity to reduce te number of candidate to the sematicaly closest ones
- Retrieve text describing the named entity

Data
- List of entities not linked: 2023018_notLinkedProcess.csv
- List of candidates as retrieved from MusicBrainz, folder: results_json/
- List of reduced candidates using Levenshtein distance, folder: candidates/ 
- Captured candidates
- Each file in candidates/ has as identifier the value of sent_n as gather form the main csv file

Requirements
- pip3 install musicbrainzngs
- pip3 install Levenshtein
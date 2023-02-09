# NER-musicbrainz
 
# Named entity recognition using MUSICBRAINZ API

Problem:
- Music personalities not identified in other databases

Approach
- Use MusicBrainz database and its API to search for entities missing
- Use musicbrainzngs python library to use the API
- Retrieve list of candidate names
- Use cosine similarity to reduce te number of candidate to the sematicaly closest ones
- Retrieve text describing the named entity

Data
- List of candidates as retrieved from MusicBrainz
- List of reduced candidates using cosine similarity
- Captured text describing entities

Requirements
- pip3 install musicbrainzngs
- pip3 install Levenshtein
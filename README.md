# dynapi
Dynalist API Extras

Installation:

`pip install dynapi`

Usage:

`export DYNALIST_API_KEY=YOUR DYNALIST API KEY`

```python
import dynapi

io = dynapi.DynalistIO()

# Alternatively:
# io.API_KEY = 'YOUR DYNALIST API KEY'
# io.set_api_key() # Hidden input

# Searching for Files
io.search_files(title='String...')

# Getting file Data
data = io.get_file(file_id='FILE_ID') # Alternative option: refresh=False
                                      # Requires set: io.CACHING = True (may eat more memory)
```

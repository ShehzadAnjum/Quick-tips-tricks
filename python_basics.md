## 📌 Naming Conventions Help

| Name        | Assumed Type                   |
| ----------- | ------------------------------ |
| `agents`    | module (lowercase)             |
| `Agent`     | class (PascalCase / CamelCase) |
| `get_agent` | function (snake\_case)         |
| `agent`     | variable (snake\_case)         |


## 🧠 General Rule in Python:

```bash
from <module> import <object>
```

This means:  
__agents__ is assumed to be a module (i.e., a .py file or package)  
__Agent__ is something defined inside that module (could be a class, function, or variable)

## Loading environment variables from .env
``` bash
import os
from dotenv import load_dotenv, find_dotenv

load_dotenv(find_dotenv())
gemini_api_key = os.getenv("GEMINI_API_KEY")

# Check if the API key is present; if not, raise an error
if not gemini_api_key:
    raise ValueError("GEMINI_API_KEY is not set. Please ensure it is defined in your .env file.")
```

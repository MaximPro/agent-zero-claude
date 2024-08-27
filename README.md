# Agent Zero - Claude 3.5 Edition

This is a modified version of the [Agent Zero](https://github.com/frdel/agent-zero) project, adapted to work with Claude 3.5 and implement caching for improved performance.

## Changes from the original project

1. Updated to use Claude 3.5 Sonnet as the default language model
2. Implemented caching to reduce redundant API calls
3. Simplified agent configuration

## Setup

1. Clone this repository
   ```
   git clone https://github.com/MaximPro/agent-zero-claude
   ```
3. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```
4. Set up your environment variables:
   - Create a `.env` file in the project root
   - Add your Anthropic API key:
     ```
     API_KEY_ANTHROPIC=your_api_key_here
     ```

## Usage

Run the main script to start the agent:

```
python main.py
```

The agent will now use Claude 3.5 Sonnet as its language model and benefit from caching to improve performance.

## Caching

The caching system stores responses from the language model to avoid making redundant API calls. This can significantly reduce the number of API requests and improve response times for repeated or similar queries.

## Configuration

You can modify the agent's configuration in the `initialize` function within `main.py`. The current setup uses minimal configuration, but you can add more parameters as needed.

## Note

This modified version focuses on using Claude 3.5 and implementing caching. Some features from the original Agent Zero project may not be fully tested with these changes. Please refer to the original project's documentation for more detailed information on available features and tools.

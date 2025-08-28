Function Calling Module Submission
1. Function Calling Example
A user writes:  
"I feel stressed and can't focus on my tasks."

Prompt to AI (with function calling):  
Use the `suggestCopingStrategy` function to analyze the user's mood and return a coping strategy.

Function definition:  
function suggestCopingStrategy(emotion: string): { suggestion: string, resources: string[] }

Expected AI Output (function call):  
{
  "function_call": {
    "name": "suggestCopingStrategy",
    "arguments": {
      "emotion": "Stressed"
    }
  }
}

Expected function response:  
{
  "suggestion": "Try a 5-minute guided breathing exercise.",
  "resources": ["Breathing Exercise Video", "Spotify: Calming Playlist"]
}
2. Explanation
Function calling in LLMs allows the AI to trigger specific backend functions based on user input. In this project, the AI detects the emotion and calls the suggestCopingStrategy function, which returns structured suggestions and resources. This makes the workflow more modular and reliable.
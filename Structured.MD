Structured Output Module Submission
A user writes:  
"I feel overwhelmed and sad today."  
Prompt to AI:  
Analyze the user's mood and return the result in structured JSON format.

Expected AI Output (Structured JSON):  
{
  "emotion": "Sad",
  "intensity": "High",
  "suggestion": "Try journaling your thoughts and listen to a calming playlist.",
  "resources": [
    "Guided journaling exercise",
    "Spotify: Calming Playlist"
  ]
}
2. Explanation
Structured output in LLMs means the AI returns data in a well-defined format (like JSON), making it easy for your app to parse and use the results. In this project, the AI is prompted to respond with a JSON object containing emotion, intensity, suggestions, and resources, ensuring consistent and machine-readable outputs.
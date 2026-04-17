---
name: fireflies-transcript
description: >
  Download the entire transcript from a Fireflies.ai call by title.
  Ensures all speakers, timestamps, and dialogues are captured.
  Saves the output as a .doc file.
version: 1.0.0
---

# Fireflies Transcript Skill

This skill allows you to retrieve a complete transcript from Fireflies.ai for a specific call and save it as a document.

## Process

### 1. Identify the Call
- Extract the call title from the user's request.
- **IMPORTANT**: If the user has not specified a call title, you MUST ask them for it before proceeding. Do not assume or default to any call name (e.g., "Jenna <> Automates" is only for your internal reference as an example).
- If multiple titles are mentioned, ask for clarification.

### 2. Search and Navigate
- Navigate to Fireflies (app.fireflies.ai/notebook).
- Search for the specific call title provided by the user.
- Click on the correct call to open the transcript view.

### 3. Extract Transcript
- Ensure the transcript is fully loaded.
- Capture:
    - Speaker names
    - Timestamps for each dialogue turn
    - Full text of the dialogue
- Do not miss anything; ensure every person said with their names and timestamps is included.

### 4. Format and Save
- Format the transcript cleanly (e.g., "[Timestamp] Speaker: Text").
- Save the final content to a file named `[Call Name].doc` (e.g., `Jenna_Automates.doc`) using the `write_to_file` tool.
- Confirm the save location to the user.

---
name: interview-template
description: >
  Fill out a structured interview template using call notes and a transcript.
  Synthesizes information from multiple sources into a final document.
  Saves the output as "Completed Interview.doc".
version: 1.0.0
---

# Interview Template Skill

This skill allows you to transform raw interview notes and call transcripts into a structured "Completed Interview" document.

## Inputs
- **Interview Notes**: Notes taken by the user during or after the call.
- **Call Transcript**: The full text of the conversation (potentially from the `fireflies-transcript` skill).

## Process

### 1. Gather Required Data
- Ensure you have both the user's notes and the call transcript.
- If either is missing, ask the user to provide them or trigger the `fireflies-transcript` skill if appropriate.

### 2. Identify the Template
- Search the workspace for an interview template document.
- **If no template is found**: Ask the user to provide the template structure or paste the template they wish to use.

### 3. Synthesize and Fill
- Map the information from the notes and transcript to the corresponding sections of the template.
- Ensure all key insights, action items, and data points are captured.
- Maintain a professional and objective tone.

### 4. Save and Deliver
- Save the completed document as `Completed Interview.doc` using the `write_to_file` tool.
- Confirm to the user that the document has been created and provide the file path.

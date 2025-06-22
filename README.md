# AI Song Generator Quiz

A simple, interactive web application that helps users create prompts for AI-generated songs through a guided quiz format.

## What it does

This quiz walks users through 8 carefully crafted questions to build a comprehensive song prompt that can be used with AI music generation tools. The questions cover:

- **Genre** - Pop, Alternative Rock, Outlaw Country, or Rap
- **Mood** - Emotional tone of the song
- **Subject** - Who or what the song is about
- **Theme** - Central message or story
- **Setting** - Where the story takes place
- **Perspective** - Point of view (first, second, third person, or duet)
- **Imagery** - Specific visual details to include
- **Chorus Style** - Type of chorus structure

After completing the quiz, users get a formatted prompt they can copy and paste into AI music generation tools like Suno, Udio, or other AI songwriting platforms.

## Features

- Clean, modern interface with smooth transitions
- Mobile-responsive design
- One-click copy to clipboard functionality
- No dependencies - pure HTML, CSS, and JavaScript

## How to use

### Quick Start (Local Development)

1. **Clone or download** this repository
2. **Install http-server** globally (if you haven't already):
   ```bash
   npm install -g http-server
   ```
3. **Navigate to the project directory**:
   ```bash
   cd song-generator
   ```
4. **Start the server**:
   ```bash
   http-server
   ```
5. **Open your browser** and go to `http://localhost:8080` (or the port shown in your terminal)

### Alternative: Direct File Opening

You can also simply open the `index.html` file directly in your web browser by double-clicking it, though using http-server is recommended for the best experience.

## Usage Instructions

1. **Start the quiz** - The page will display the first question automatically
2. **Answer each question** - Click on your preferred option from the multiple choices
3. **Complete all 8 questions** - The quiz will automatically progress through each question
4. **Get your prompt** - After the final question, you'll see a formatted song prompt
5. **Copy the prompt** - Click "Copy to Clipboard" to copy the generated prompt
6. **Use with AI tools** - Paste the prompt into your favorite AI music generation platform

## Example Output

After completing the quiz, you might get a prompt like:

```
Write a Pop Song that is joyful and uplifting, told from first person ("I").

It's about a best friend, with a theme of celebrating success.

Set in a big city at night, include imagery like fireworks lighting up the sky and a chorus that is catchy and repetitive.
```

## Technical Details

- **Framework**: Vanilla JavaScript (no dependencies)
- **Styling**: CSS with Google Fonts (Inter and Pacifico)
- **Compatibility**: Works in all modern browsers
- **File Size**: Single HTML file (~6KB)

## Customization

You can easily customize the quiz by editing the `quizQuestions` array in the JavaScript section. Each question object contains:

- `q`: The question text
- `key`: The variable name for storing the answer
- `options`: Array of possible answers

## License

This project is open source and available under the MIT License.

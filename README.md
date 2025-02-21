# Kala - A CLI app to track time on tasks

## What is this?

This started as a way to track time I was spending on user stories at work. Every user story was budgeted for certain hours and if you were going overboard that was bad, worse if you couldn't finish the story in the sprint.

Naturally, that happened to me more often that I'd like to remember.

This app is a generalised version of the tool I'd come to use at work. This app is short and simple. Add a task and start working on it. It'll keep time how long you've been working on it.

I could have used some time tracking app already available but I wanted something I can run in the terminal, something unobtrusive, and something simple.

This project was also a good excuse to dip my feet into Go.

The name is from [Kāla](https://en.wikipedia.org/wiki/K%C4%81la), ChatGPT wasn't very helpful with naming. I didn't want something too boring.
I like one word names for apps, I just picked this because it is in fact descriptive, albeit in a different language, and it wouldn't cause naming conflicts.

## Installation

Follow these steps to build Kala from source:  

1. **Ensure you have Go installed**  
   - Download and install Go from [golang.org](https://go.dev/dl/).  
   - Verify installation:  
     ```sh
     go version
     ```

2. **Clone the repository**  
   ```sh
   git clone https://github.com/yourusername/kala.git
   cd kala
   ```

3. **Build binary**
    ```sh
    go build -o kala
    ```

4. **Add to PATH**
You can move the binary anywhere you like. I have been keeping it in `~/.local/bin` and the sqlite database in `~/.local/share/kala/`. If you'd like the same:
    ```sh
    mv kala ~/.local/bin/
    ```

5. **Ensure it's all good**
    ```sh
    kala --help
    ```

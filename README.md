<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>AI & Gamer Hub</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <header>
    <h1>Welcome to AI & Gamer Hub</h1>
    <p>Your one-stop site for gaming, coding, and AI resources</p>
  </header>

  <main>
    <section>
      <h2>🎮 Gamer Tools</h2>
      <ul>
        <li><a href="https://obsproject.com/" target="_blank">OBS Studio - Game Recording</a></li>
        <li><a href="https://geforce.com/geforce-experience" target="_blank">NVIDIA GeForce Experience</a></li>
        <li><a href="https://store.steampowered.com/" target="_blank">Steam - Game Library</a></li>
      </ul>
    </section>

    <section>
      <h2>🔍 Research</h2>
      <ul>
        <li><a href="https://scholar.google.com/" target="_blank">Google Scholar</a></li>
        <li><a href="https://www.sciencedirect.com/" target="_blank">ScienceDirect</a></li>
        <li><a href="https://www.arxiv.org/" target="_blank">arXiv - Research Papers</a></li>
      </ul>
    </section>

    <section>
      <h2>💻 Coding Websites</h2>
      <ul>
        <li><a href="https://github.com/" target="_blank">GitHub</a></li>
        <li><a href="https://codepen.io/" target="_blank">CodePen</a></li>
        <li><a href="https://replit.com/" target="_blank">Replit</a></li>
      </ul>
    </section>

    <section>
      <h2>🧠 ChatGPT & AI Tools</h2>
      <ul>
        <li><a href="https://chat.openai.com/" target="_blank">ChatGPT</a></li>
        <li><a href="https://openai.com/research" target="_blank">OpenAI Research</a></li>
        <li><a href="https://www.perplexity.ai/" target="_blank">Perplexity AI</a></li>
      </ul>
    </section>

    <section>
      <h2>🤖 About AI</h2>
      <p>Artificial Intelligence (AI) is the simulation of human intelligence in machines. It powers tools like ChatGPT, image generation, self-driving cars, and more. AI is transforming every industry from education to healthcare to gaming.</p>
    </section>
  </main>

  <footer>
    <p>© 2025 AI & Gamer Hub. Built by meronepal-cpu.</p>
  </footer>
</body>
</html>
body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
  background: #0d1117;
  color: white;
}
header {
  background-color: #1f6feb;
  padding: 20px;
  text-align: center;
  color: white;
}
main {
  padding: 20px;
}
section {
  margin-bottom: 30px;
  background: #161b22;
  padding: 15px;
  border-radius: 8px;
}
h1, h2 {
  color: #58a6ff;
}
a {
  color: #8ab4f8;
  text-decoration: none;
}
a:hover {
  text-decoration: underline;
}
footer {
  text-align: center;
  padding: 10px;
  background: #161b22;
  color: #8b949e;
}
import java.util.Scanner;
import java.util.Random;

public class GuessNumber {
    public static void main(String[] args) {
        Random rand = new Random();
        int numberToGuess = rand.nextInt(100) + 1;
        Scanner input = new Scanner(System.in);
        int guess = 0;

        System.out.println("🎮 Guess the number between 1 and 100:");

        while (guess != numberToGuess) {
            System.out.print("Enter your guess: ");
            guess = input.nextInt();

            if (guess < numberToGuess) {
                System.out.println("Too low!");
            } else if (guess > numberToGuess) {
                System.out.println("Too high!");
            } else {
                System.out.println("🎉 You got it!");
            }
        }

        input.close();
    }
}

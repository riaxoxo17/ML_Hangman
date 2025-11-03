Hangman AI — HMM + DQN Hybrid Agent
📘 Overview

This project implements an intelligent Hangman-playing agent that combines Hidden Markov Models (HMM) and Deep Q-Networks (DQN) for optimal letter prediction.
It demonstrates a hybrid AI system that merges probabilistic modeling with reinforcement learning to improve the success rate on unseen words.

⚙️ Features

🧩 HMM-based language model for probabilistic letter prediction

🤖 DQN-based reinforcement agent for dynamic decision-making

🎯 Reward shaping to encourage progress and discourage repeated/wrong guesses

🔁 Epsilon-greedy exploration with adaptive decay

📊 Comprehensive evaluation on 2000-word test set

🚀 Setup & Execution
1️⃣ Install Dependencies
pip install numpy torch tqdm matplotlib reportlab

2️⃣ Run the Notebook

Open ML_hackathon_final.ipynb in Jupyter Notebook or Google Colab.

3️⃣ Upload Corpus

When prompted, upload a large English text file, such as:

corpus.txt


Preferably containing around 50,000 words for meaningful HMM statistics.

4️⃣ Train the Model

Run all notebook cells sequentially until training completes.
The training combines HMM priors with DQN learning, optimizing letter prediction and reducing wrong guesses.

5️⃣ Evaluate the Model

After training, run the final evaluation cell:

final_results = evaluate_agent(agent, test_words, num_games=2000)

6️⃣ Test a Single Word (Demo)

You can demo the trained agent on a custom word:

play_single_game(agent, "elephant")

🧠 Project Summary

This project demonstrates that combining language modeling (HMM) with reinforcement learning (DQN) creates a more powerful Hangman agent.
The HMM provides structure and priors, while the DQN learns adaptively through experience.
Together, they form a hybrid AI system capable of balancing exploration, exploitation, and linguistic intuition.

import random

text = """
ProDigy Infotech is a leading IT company. It provides software development, training, and consultancy services.
We focus on quality solutions and innovative technologies. Our team works with dedication and excellence.
"""

words = text.split()
markov_chain = {}

for i in range(len(words) - 1):
    key = words[i]
    next_word = words[i + 1]
    if key in markov_chain:
        markov_chain[key].append(next_word)
    else:
        markov_chain[key] = [next_word]

def generate_text(chain, length=30):
    word = random.choice(list(chain.keys()))
    result = [word]
    for _ in range(length - 1):
        if word in chain:
            word = random.choice(chain[word])
        else:
            word = random.choice(list(chain.keys()))
        result.append(word)
    return " ".join(result)

generated_text = generate_text(markov_chain, 50)
print("Generated Text:\n")
print(generated_text)

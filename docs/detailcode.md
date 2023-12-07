import random

# Number of piles
num_piles = 9

# Number of tokens in each pile
tokens_per_pile = 21000000

# Communicate randomly between piles
for pile in range(num_piles):
    for _ in range(num_piles):
        if pile != _:
            communication_tokens = random.randint(1, tokens_per_pile)
            print(f"Pile {pile + 1} communicates {communication_tokens} tokens to Pile {_ + 1}")

# Vigenere-Algorithm-Cryptography-python-project
tep 1: Setup

Alphabet: abcdefghijklmnopqrstuvwxyz

Key: happycoding → repeated for each letter in the text.

We skip spaces (they are added as-is).

Step 2: Trace each character
First word: "mrttaqrhknsw"

'm' (index=12), key 'h' (offset=7)
→ (12 - 7) % 26 = 5 → 'f'

'r' (17), key 'a' (0)
→ (17 - 0) % 26 = 17 → 'r'

't' (19), key 'p' (15)
→ (19 - 15) % 26 = 4 → 'e'

't' (19), key 'p' (15)
→ (19 - 15) % 26 = 4 → 'e'

'a' (0), key 'y' (24)
→ (0 - 24) % 26 = 2 → 'c'

'q' (16), key 'c' (2)
→ (16 - 2) % 26 = 14 → 'o'

'r' (17), key 'o' (14)
→ (17 - 14) % 26 = 3 → 'd'

'h' (7), key 'd' (3)
→ (7 - 3) % 26 = 4 → 'e'

'k' (10), key 'i' (8)
→ (10 - 8) % 26 = 2 → 'c'

'n' (13), key 'n' (13)
→ (13 - 13) % 26 = 0 → 'a'

's' (18), key 'g' (6)
→ (18 - 6) % 26 = 12 → 'm'

'w' (22), key 'h' (7, key repeats)
→ (22 - 7) % 26 = 15 → 'p'

✅ First word = "freecodecamp"

Space → " "

(stays as-is)

Second word: "ih puggrur"

'i' (8), key 'a' (0, key repeats at position 2)
→ (8 - 0) % 26 = 8 → 'i'

'h' (7), key 'p' (15)
→ (7 - 15) % 26 = 18 → 's'

(space stays same)

'p' (15), key 'p' (15)
→ (15 - 15) % 26 = 0 → 'a'

'u' (20), key 'y' (24)
→ (20 - 24) % 26 = 22 → 'w'

'g' (6), key 'c' (2)
→ (6 - 2) % 26 = 4 → 'e'

'g' (6), key 'o' (14)
→ (6 - 14) % 26 = 18 → 's'

'r' (17), key 'd' (3)
→ (17 - 3) % 26 = 14 → 'o'

'u' (20), key 'i' (8)
→ (20 - 8) % 26 = 12 → 'm'

'r' (17), key 'n' (13)
→ (17 - 13) % 26 = 4 → 'e'

✅ Second word = "is awesome"

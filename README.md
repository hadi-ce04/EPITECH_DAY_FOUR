# EPITECH_DAY_FOUR
# 🕵️ Vigenère Cipher Breaker

An automated cryptanalysis tool designed to break secret codes encrypted with the Vigenère Cipher without knowing the key in advance.

![Vigenère Cipher Table](https://pages.mtu.edu/~shene/NSF-4/Tutorial/VIG/FIG-VIG-Table.jpg)

---

### How It Works

1. **Groups Interleaved Letters:** A Vigenère cipher uses a repeating key word to shift letters in a cycle. The program splits encrypted text into smaller chunks so that every letter in a single chunk shares the exact same secret key shift.

![Cipher Disk Wheel](https://encrypted-tbn0.gstatic.com/licensed-image?q=tbn:ANd9GcS65yq39JEsFm1-2eVUN6crLkshdYXDl2SjRHywf3hSxR-1nbzC8jVZTFTZ8B7qG4IuakgO0OgxYRmYpFCb1iTMZON7YmsisGpl)

2. **Performs Frequency Analysis:** In normal English, the letter **'E'** appears far more frequently than any other letter.

![English Letter Frequency Graph](https://pi.math.cornell.edu/~mec/2003-2004/cryptography/subs/frequency.jpg)

3. **Reconstructs the Key:** For each chunk of text, the program finds the most frequent character, assumes it was originally an **'E'**, and calculates how many steps it was shifted. It then stitches those shifts together to reveal the secret password.

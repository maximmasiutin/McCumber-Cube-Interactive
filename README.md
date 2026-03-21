# Interactive Information Security Visualizations

Interactive HTML pages for teaching information security concepts. All pages support English, Romanian, and Russian. CSS and JavaScript are inline with no external libraries required. Optional image files enhance the RSA page but are not required (emoji fallbacks are provided).

## Interactive Pages

### McCumber Cube

**File:** [mccumber-cube-interactive-index.html](mccumber-cube-interactive-index.html)

Interactive 3D visualization of the McCumber Cube information security framework, introduced by John McCumber in 1991. The model maps 27 cells (3 x 3 x 3) across three dimensions:

1. **Security Goals (CIA Triad)**: Confidentiality, Integrity, Availability
2. **Data States**: At Rest, In Transit, In Processing
3. **Countermeasures**: Technology, Policies & Practices, Education & Training

Features:
- Rotating 3D cube with clickable cells
- Dimension selector with bidirectional highlighting across the cube and the reference table
- Detail panel showing the security requirement for each of the 27 cell combinations
- Full 27-cell reference matrix with concrete examples

### OSI Reference Model

**File:** [osi-model-interactive.html](osi-model-interactive.html)

Interactive 7-layer OSI (Open Systems Interconnection) reference model visualization.

Features:
- Color-coded layers with protocol listings
- Mnemonic phrases for memorizing layer order (bottom-to-top and top-to-bottom)
- Hover effects for layer exploration

### RSA Algorithm

**File:** [rsa-algorithm-interactive.html](rsa-algorithm-interactive.html)

Interactive RSA cryptography lab with the classic Alice-Bob scenario for key generation, encryption, and decryption.

Features:
- Key generation: enter primes p and q, compute modulus n, totient t, public exponent e, private exponent d
- Encryption: Bob encrypts message m with Alice's public key (n, e)
- Decryption: Alice decrypts ciphertext c with her private key (n, d)
- "Send public key to Bob" button transfers keys between panels
- "Random primes" button for quick demonstration
- Input validation with real-time feedback (primality, coprimality, m < n bounds)
- Step-by-step instructions with field-focus highlighting
- Fireworks animation on successful decryption matching original plaintext
- Emoji avatar fallback when character images are not present

## Usage

Open any HTML file directly in a modern browser. All CSS and JavaScript are inline. The RSA page optionally loads alice.jpg and bob.jpg if present in the same directory, falling back to emoji avatars otherwise.

## Fonts

The pages reference Helvetica Neue World (body text, supports Latin + Cyrillic), Helvetica Now Display (headings), and Helvetica (fallback) by their installed system names. If these fonts are not installed, the pages fall back through Helvetica Neue, Segoe UI, and standard system sans-serif fonts.

## Context

Created for the Information Security Technologies course at the Technical University of Moldova.

## License

This project is licensed under the GNU General Public License v3.0. See [LICENSE](LICENSE) for details.

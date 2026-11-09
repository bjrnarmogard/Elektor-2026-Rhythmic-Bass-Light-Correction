# 🚀 Official Engineering Correction: Elektor Magazine (2026)

This repository documents an official technical correction submitted to and published in **Elektor Magazine** regarding the article *"Rhythmic Bass Light"* by Giuseppe La Rosa in **Circuit Special 2026 (No. 547)**.

## 🔍 The Discrepancy & Mathematical Verification
The article claimed a low-pass filter cutoff frequency of **70 Hz** with $R_4 = 0\ \Omega$, using $R_3 = 22\text{ k}\Omega$ and $C_3 = 10\text{ nF}$. My independent verification calculated the actual frequency as:

$$F_c = \frac{1}{2\pi \times 22,000\ \Omega \times 10\text{ nF}} \approx 724\text{ Hz}$$

## 🏆 Official Editorial Approval (No. 549)
My correction was verified and published in the **November & December 2026** edition (No. 549) with official confirmation from Editor-in-Chief Roberto Armani, who acknowledged the typo and confirmed the value should have been **≈ 700 Hz**.

**Reported and documented by:**  
Bjørnar Mogård (Norway)  
*Hardware Integrity & Electronics Review*

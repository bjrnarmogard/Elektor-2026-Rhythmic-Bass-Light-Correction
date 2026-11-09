# Elektor-2026-Rhythmic-Bass-Light-Correction

# 🚀 Official Engineering Correction: Elektor Magazine (Circuit Special 2026)

This repository documents an official technical correction and errata identified, calculated, and verified in **Elektor Magazine (Circuit Special 2026, p. 42)**.

During a detailed mathematical analysis of the published audio circuits, I discovered a significant calculation error regarding the filter dimensioning in an official article. My independent calculations were submitted to Elektor Labs, formally approved by Editor-in-Chief Roberto Armani, and published internationally under the *Errata / Letters* section.

---

## 🔍 The Discovered Errata: "Rhythmic Bass Light" (Page 42)

In the technical article *"Rhythmic Bass Light"* written by Giuseppe La Rosa (circuit reference 260142), the text describes the active low-pass filter stage built around the **LM358D operational amplifier (IC1A)**. 

### The Discrepancy in the Magazine:
The printed article stated that when the trimmer resistor $R_4$ is shorted ($0\ \Omega$), the cutoff frequency of the low-pass filter is **approximately 70 Hz**. 

![Original Text Error](errata_magazine.png)
*Figure 1: The original paragraph on page 42 incorrectly stating a 70 Hz cutoff frequency.*

### My Mathematical Analysis & Verification:
By analyzing the schematic, the fixed resistance in the feedback loop is $R_3 = 22\text{ k}\Omega$ and the filter capacitor is $C_3 = 10\text{ nF}$. Using the standard cutoff frequency formula for an active inverting filter configuration:

$$F_c = \frac{1}{2\pi \times 22,000\ \Omega \times 10\text{ nF}} \approx 724\text{ Hz}$$

The printed value of 70 Hz was mathematically impossible with the given component values (it would have required a $100\text{ nF}$ capacitor instead). 

---

## 🏆 Official Editorial Approval & Publication

The international editorial board verified my breakdown and published my letter alongside the official confirmation in the next column:

![Official Publication Svar](elektor_reply.png)
*Figure 2: My published letter and the official confirmation from Elektor's Editor-in-Chief.*

> *"Thanks for your report. Indeed, it's a typo. The indicated component values are correct: The text should have reported '≈ 700 Hz'."*
> — **Roberto Armani**, Editor-in-Chief, Elektor Magazine

This repository stands as a testament to rigorous hardware verification and cross-examination of published material against raw datasheet physics.

**Reported and documented by:**  
Bjørnar Mogård (Norway)  
*Hardware Integrity & Electronics Review*

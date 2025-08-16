# Strong-Password-Creation-Evaluation

## Objective
To create different sample passwords (weak → strong), test them using free password strength checkers, and analyze what makes a password secure.

## Environment
- **Operating System:** Windows 10
- **Tools Used:** Wireshark not needed here; Free password strength checkers:
  - https://passwordmeter.com
  - https://howsecureismypassword.net (or any other)

## Steps Performed
1. Created 4 candidate passwords with varying complexity.
2. Evaluated each on two password strength checkers.
3. Collected results (length, feedback, strength score).
4. Saved screenshots of results in `/screenshots/`.
5. Analyzed trends: why some passwords are weak/strong.
6. Summarized best practices and key concepts.

## Candidate Passwords Tested
(Labels only; do not reuse these exact samples in real life)
- **P1:** `99985623` → short, lowercase only
- **P2:** `qwert123456` → lowercase + digits
- **P3:** `Zwety56YHNasm` → mixed case + digits
- **P4:** `{or66igVP,Y37]75[b!` → mixed + symbol

## Results (Snapshot from results.csv)
| Password | Length | Tool A Score | Notes |
|----------|--------|--------------|----------------------------|
| P1       | 8      | 15%          | Too short, dictionary word |
| P2       | 11     | 30%          |  Slightly better, still weak |
| P3       | 13     | 86%          | Mixed case helps |
| P4       | 19     | 100%         | Symbol adds strength |

## Key Findings
- **Length is most important** → strength grows exponentially with more characters.
- **Character variety helps**, but predictable patterns (`Name@123`) still weak.
- **Dictionary words are risky** even if mixed with numbers.
- **Passphrases** (multiple random words) are strong + easier to remember.
- **Random 16–20+ chars** are strongest but need a password manager.

## Best Practices
- Use **14+ chars minimum**, aim for 16–20.
- Combine **upper/lowercase, numbers, and symbols** in unpredictable ways.
- Avoid dictionary words, names, dates, or patterns.
- Prefer **unique password per site** (no reuse).
- Enable **MFA (Multi-Factor Authentication)**.
- Use a **password manager** for random long ones.
- For memorability, use **passphrases** with unrelated words.


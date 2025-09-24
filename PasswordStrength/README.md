# Password Strength Meter

This repository contains a **Password Strength Meter** React component and a custom hook for measuring password strength.

It is a **reusable component** that can be easily integrated into any React project to give users real-time feedback about the strength of their passwords.

---

## 📂 Files

### 1. `src/hooks/usePasswordStrength.js`

A **custom React hook** that calculates the strength of a given password and returns:

| Key       | Type   | Description                                       |
| --------- | ------ | ------------------------------------------------- |
| `score`   | number | Password strength score (0–5)                     |
| `percent` | number | Percentage for visual strength bar (0–100)        |
| `label`   | string | Strength label (`Weak`, `Fair`, `Good`, `Strong`) |
| `color`   | string | Color code for strength indicator                 |

**Usage:**

```js
import usePasswordStrength from "../hooks/usePasswordStrength";

const { score, percent, label, color } = usePasswordStrength(password);
```

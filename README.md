# Before You Speak

An interactive React component based on the **Abhaya Sutta (Majjhima Nikaya 58)** - the Buddha's five-gate framework for deciding whether, when, and how to speak.

![Buddhist speech framework](https://img.shields.io/badge/source-Abhaya%20Sutta%20MN%2058-8B5E3C?style=flat-square)
![React](https://img.shields.io/badge/React-18%2B-61DAFB?style=flat-square&logo=react)

## What It Does

Before speaking, the Tathagata passes each word through five qualities:

1. **True** - Not assumption or imagination
2. **Factual** - Verifiable, not hearsay
3. **Beneficial** - Will it genuinely help the person?
4. **Endearing** - Is it welcome to hear?
5. **Agreeable** - Does the person accept it?

The component walks you through these gates interactively and returns one of four verdicts:

| Result | Meaning |
|---|---|
| Noble Silence | Don't say it |
| Noble Silence (sweet) | True and likeable, but not helpful right now |
| Speak - Wait for the Right Moment | Beneficial but hard to hear; wait for receptivity |
| Speak - With Right Timing | All five gates open; still wait for the right moment |

## Usage

Drop it into any React project:

```bash
cp speech-framework.jsx src/components/
```

```jsx
import SpeechFramework from './components/speech-framework';

export default function App() {
  return <SpeechFramework />;
}
```

No dependencies beyond React itself.

## The Decision Matrix

These are the six cases laid out in the sutta, verbatim:

| # | True & Factual | Beneficial | Endearing & Agreeable | Action |
|---|---|---|---|---|
| 1 | No | No | No | Does not speak |
| 2 | Yes | No | No | Does not speak |
| 3 | Yes | Yes | No | Speaks with right timing |
| 4 | No | No | Yes | Does not speak |
| 5 | Yes | No | Yes | Does not speak |
| 6 | Yes | Yes | Yes | Speaks with right timing |

The key insight: only cases 3 and 6 result in speaking - and even then, only at the right time. Case 4 is easy to miss: something that feels good to say but is untrue is still silence.

> *"Why does the Tathagata exercise a sense of time? Because the Tathagata has sympathy for living beings."*
> — Abhaya Sutta, MN 58

## Source

**Abhaya Sutta · Majjhima Nikaya 58**

The sutta records a conversation between Prince Abhaya and the Buddha. Abhaya was sent by a rival teacher to trap the Buddha with a two-horned question: "Does the Tathagata say words that are unendearing to others?" Either answer would box him in.

The Buddha's response doesn't fit either horn - he lays out six specific cases that show when he speaks and when he doesn't. The principle: truth and benefit are non-negotiable. Pleasantness alone is never a reason to speak. And even when all conditions are met, he still waits for the right moment - out of sympathy, not strategy.

## License

MIT

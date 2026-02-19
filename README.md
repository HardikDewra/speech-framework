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

| Qualities | Action |
|---|---|
| Untrue | Does not speak |
| True + factual, but unbeneficial | Does not speak |
| True + factual + beneficial, but unwelcome | Speaks with right timing |
| True + factual + unbeneficial, but endearing | Does not speak |
| All five present | Speaks with right timing |

> *"Why does the Tathagata exercise a sense of time? Because the Tathagata has compassion for all living beings."*
> — Abhaya Sutta, MN 58

## Source

**Abhaya Sutta · Majjhima Nikaya 58**

The sutta records a conversation between the Buddha and Prince Abhaya, in which the Buddha explains the five qualities he considers before speaking any word - and why even true, beneficial words are held back until the right moment.

## License

MIT

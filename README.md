# 🔄 String Inverter

> A lightweight, zero-dependency JavaScript utility that reverses any string instantly.

---

## ✨ Features

- ⚡ **Instant reversal** — runs in O(n) time
- 🪶 **Zero dependencies** — pure vanilla JavaScript
- 🔡 **Unicode safe** — handles letters, numbers, symbols, and spaces
- 📦 **Tiny footprint** — just 3 lines of code

---

## 📦 Installation

Clone the repo or copy the function directly into your project:

```bash
git clone https://github.com/lorddrago12/String-Inverter.git
cd String-Inverter
```

---

## 🚀 Usage

```js
function reverseString(str) {
  const reversed = str.split("").reverse().join("");
  return reversed;
}

reverseString("hello");       // → "olleh"
reverseString("JavaScript");  // → "tpircSavaJ"
reverseString("12345");       // → "54321"
reverseString("racecar");     // → "racecar"
reverseString("");            // → ""
```

---

## 🧪 Examples

| Input         | Output        |
|---------------|---------------|
| `"hello"`     | `"olleh"`     |
| `"world"`     | `"dlrow"`     |
| `"JavaScript"`| `"tpircSavaJ"`|
| `"12345"`     | `"54321"`     |
| `"racecar"`   | `"racecar"`   |
| `""`          | `""`          |

---

## 🛠️ How It Works

```
"hello"
   │
   ▼
split("")  →  ["h", "e", "l", "l", "o"]
   │
   ▼
reverse()  →  ["o", "l", "l", "e", "h"]
   │
   ▼
join("")   →  "olleh"
```

1. **`split("")`** — breaks the string into an array of individual characters
2. **`reverse()`** — reverses the array in place
3. **`join("")`** — joins the characters back into a single string

---

## ⚠️ Limitations

- Does not correctly handle **emoji** or multi-codepoint Unicode characters (e.g., `"👨‍👩‍👧"`)
- For emoji/Unicode support, consider using the [Intl.Segmenter](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Intl/Segmenter) API or the [`grapheme-splitter`](https://www.npmjs.com/package/grapheme-splitter) library

---

## 🤝 Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request.

1. Fork the repository
2. Create your feature branch: `git checkout -b feature/my-feature`
3. Commit your changes: `git commit -m 'Add my feature'`
4. Push to the branch: `git push origin feature/my-feature`
5. Open a Pull Request

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

<p align="center">Made with ❤️ and vanilla JavaScript</p>

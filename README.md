# Malaysian IC Formatter

A simple browser tool that normalizes Malaysian Identity Card (MyKad) numbers to the standard format:

```text
XXXXXX-XX-XXXX
```

## Why

Excel and other sources often mix formats — some ICs already have dashes (`591018-13-5745`), others are plain 12-digit strings (`880923525170`). Paste either; this tool outputs a consistent list you can copy back into a spreadsheet.

## Usage

1. Open [`ic-formatter.html`](ic-formatter.html) in a browser  
   (or via Laragon: `http://formatic.test/ic-formatter.html`)
2. Paste your IC list into the text box (one per line, or separated by commas / tabs)
3. Click **Format** (or wait — it also formats as you paste/type)
4. Click **Copy result** and paste back into Excel

### Examples

| Input | Output |
|--------|--------|
| `591018-13-5745` | `591018-13-5745` |
| `880923525170` | `880923-52-5170` |
| `750408135930` | `750408-13-5930` |

Invalid rows (not exactly 12 digits after stripping non-digits) are left unchanged.

## Files

- `ic-formatter.html` — single-file HTML + CSS + JavaScript (no server or build step required)

## License

Free to use and modify.
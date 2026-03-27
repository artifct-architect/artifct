# Quickstart

## Browser (fastest)

1. Open `app/capsule_creator.html`
2. Drop a file
3. Generate capsule
4. Open artifact

---

## CLI

```bash
pip install cryptography

python cli/capsule.py keygen
python cli/capsule.py seal file.txt --author "You"
python cli/capsule.py verify file.txt.cap
```

---

## Explorer

```bash
python explorer/capsule_lineage_explorer.py examples
```

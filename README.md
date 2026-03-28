# (DEMO) Capsule

Self-verifying digital artifacts.

Capsules carry their own identity, integrity, and lineage —
and can be verified offline, forever.

---

[Read the Founder Record](./FOUNDER_RECORD.md)

---

👉 [Open Example Artifact](./examples/example_artifact.html)

---

## Try it in 2 minutes

### Option 1 — No install (recommended)

1. Download `app/capsule_creator.html`
2. Open it in your browser
3. Drop in any file
4. Click **Create Capsule**
5. Open the generated artifact

---

### Option 2 — CLI

```bash
pip install cryptography

python cli/capsule.py keygen
python cli/capsule.py seal file.txt --author "You"
python cli/capsule.py verify file.txt.cap
```

---

## Example

* Open: `examples/example_artifact.html`
* Inspect a real capsule
* Verify it offline

---

## What is a Capsule?

A capsule is a file that proves itself.

It includes:

* payload (the file itself)
* SHA-256 hash (integrity)
* author
* public key
* cryptographic signature
* optional parent (lineage)

No servers. No APIs. No trust required.

---

## Lineage

Capsules can reference a parent.

This creates:

* branches
* histories
* artifact trees

Use the explorer:

```bash
python explorer/capsule_lineage_explorer.py examples
```

---

## Trust Model

Verification is:

* deterministic
* local
* offline

Everything needed to verify a capsule is inside it.

---

## Project Structure

```
/app        → browser capsule creator
/cli        → reference CLI tools
/explorer   → lineage + archive tools
/examples   → demo capsules
/docs       → concept + documentation
```

---

## Roadmap

* capsule.v1 schema
* identity layers
* hosted registry
* discovery tools
* collaboration features

---

## License

This project defines an open, verifiable artifact format.

Reference tools are provided for adoption and experimentation.

The broader ecosystem (identity, discovery, platform services)
will evolve separately.

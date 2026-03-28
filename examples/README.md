# Examples

This folder contains sample capsules and generated artifacts.

## Files

* `example.cap`
  A raw capsule file

* `example_artifact.html`
  A standalone viewer for the capsule

## How to use

### Open artifact (no setup)

Just open the HTML file in your browser.

### Verify manually

```bash
python ../cli/capsule.py verify example.cap
```

### Explore lineage

```bash
python ../explorer/capsule_lineage_explorer.py .
```

## Additional Example

- `minimal_example.cap`  
  A minimal capsule for quick inspection

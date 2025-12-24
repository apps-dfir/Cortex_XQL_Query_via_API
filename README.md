# Cortex XQL via Public API

Minimal Jupyter notebook for running **XSIAM XQL** through the **Public API** and working with the results locally.

This is intentionally small and opinionated. It solves one problem: getting XQL results out of the UI and into a notebook where you can actually work with them.

---

## What this is

- Runs existing XQL outside the XSIAM UI
- Pulls results into a pandas DataFrame
- Automatically switches to streaming for large result sets
- Designed to be read, modified, and extended

That’s it.

---

## What this is not

- Not a framework
- Not a scheduler
- Not a detection pack
- Not production automation

It’s just a working **API → notebook bridge**.

---

## How it behaves

- Uses `get_query_results` for smaller result sets
- Falls back to the stream endpoint when results exceed limits
- Downloads results locally before loading them into memory
- Leaves analysis, visualization, and scheduling up to you

No magic, no abstractions.

---

## Context

This repository is paired with a short walkthrough that explains **why** this exists and how the pieces fit together:

**Blog walkthrough:**  
[Running XSIAM XQL via the Public API from a Jupyter notebook](https://apps-ir.com/run-cortex-xsiam-xql-hunts-via-the-public-api-from-a-jupyter-notebook-1151cb225d50)

The blog covers design decisions and edge cases.  


---

## Notes

- Expect rough edges
- Expect to tweak things for your environment
- If something breaks or feels off, that’s useful feedback

This will evolve as I use it more.

---

## License

MIT
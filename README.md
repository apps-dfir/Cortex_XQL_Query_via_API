# Cortex XQL via Public API

Minimal Jupyter notebook for running **XSIAM XQL** through the **Public API** and working with the results locally.

---

## What this is

- Runs existing XQL outside the UI  
- Pulls results into a pandas DataFrame  
- Handles large result sets via the stream endpoint  

That’s it.

---

## What this is not

- Not a framework  
- Not a scheduler  
- Not a detection pack  

Just a working API → notebook bridge.

---

## Notes

- Uses `get_query_results` for small result sets  
- Switches to streaming automatically when required  
- Results are loaded locally for analysis or export  

---

## Context

For background, design decisions, and a walkthrough, see the accompanying blog post:

**https://apps-ir.com/run-cortex-xsiam-xql-hunts-via-the-public-api-from-a-jupyter-notebook-1151cb225d50**

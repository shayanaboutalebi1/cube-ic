# Integration Instructions for cube-ic

1. Unzip the archive at the root of your local clone.
2. Copy files into the repo:
   cp -r schemas templates iv7_automated_framework.md README_ADDITION.md instructions.md /path/to/cube-ic/
3. Commit:
   git add schemas templates iv7_automated_framework.md README_ADDITION.md instructions.md
   git commit -m "Add iV7 Automated Truth-Backfill addition"
   git push origin main
4. Create data folders as needed: data/raw_events, data/normalized_claims, data/evidence_index
5. Use templates/backfill_brief_template.md for each UNSTABLE claim.

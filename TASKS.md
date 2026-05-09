# Proposed Maintenance Tasks

1. **Typo fix task**
   - Fix the repository name typo in `README.md` where `ubiquitous-memory` is split into `ubiquitous-mem` and `ory`.
   - **Why:** The current text appears as broken fragments and is hard to read/copy.
   - **Acceptance criteria:** The repository name is spelled continuously as `ubiquitous-memory` everywhere in the file.

2. **Bug fix task**
   - Repair broken Git remote URLs in `README.md` by removing the accidental line breaks that split `https://github.com/rananisarsb51214-web/ubiquitous-memory.git`.
   - **Why:** Copy-pasting the current URL fails because the string is split across lines.
   - **Acceptance criteria:** All Git URLs are valid clickable/copyable full URLs that work with `git clone`.

3. **Documentation discrepancy task**
   - Rewrite `README.md` to match an expected project README structure (title, setup instructions, usage, and repository link) instead of the current duplicated and malformed URL-only content.
   - **Why:** The file is currently duplicated and does not provide actual project documentation.
   - **Acceptance criteria:** README has one clear project title and consistent sections with no duplicate malformed blocks.

4. **Test improvement task**
   - Add a markdown/content lint test (e.g., markdownlint or a small CI script) that checks for malformed URLs and duplicated first-line blocks in `README.md`.
   - **Why:** Prevents future regressions of broken links and accidental duplication.
   - **Acceptance criteria:** CI fails when a URL is broken by whitespace/newlines or when duplicate header/link blocks are introduced.

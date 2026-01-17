# 🤖 Frontier AI Research Jobs Tracker

A chronological Git repository tracking AI Research Engineer job postings across top frontier AI labs:
- **Anthropic**
- **Google DeepMind**
- **OpenAI**
- **X.ai**
- **Thinking Machines**
- **ByteDance Seed**

Reconstructed from **259 updates** (`neolab_all_emails.csv`) between **January 16, 2026** and **November 1, 2026**.

## 📁 Repository Structure
- **[`jobs.md`](jobs.md)** — The active AI research job listings snapshot. Updated in each of the 259 chronological commits to track content changes over time.
- **[`neolab_all_emails.csv`](neolab_all_emails.csv)** — The raw historical dataset containing all 259 email alerts from the AI Jobs Scraper.

## 🔍 How to Track Content Changes Over Time
Use standard Git commands to explore how job postings, requirements, and hiring volume evolved over time:

### 1. View Recent Changes
```bash
# View the changes introduced in the latest update
git diff HEAD~1 jobs.md

# View changes between any two commits or updates
git diff <commit-A> <commit-B> jobs.md
```

### 2. View Timeline & History
```bash
# View chronological commit history
git log --oneline

# View commit history with diffs
git log -p -2 jobs.md
```

### 3. Search Changes for a Specific Lab
```bash
# Track all changes affecting Anthropic
git log -S "Anthropic" -p jobs.md

# Track all changes affecting DeepMind
git log -S "DeepMind" -p jobs.md

# Track all changes affecting OpenAI
git log -S "OpenAI" -p jobs.md
```

### 4. Search for Specific Roles or Keywords
```bash
# Track when Reinforcement Learning roles were added or removed
git log -S "Reinforcement Learning" -p jobs.md

# Track when Frontier or Pre-training roles changed
git log -S "Pre-training" -p jobs.md
```

### 5. Line Attribution & Blame
```bash
# See which commit and date introduced each job listing
git blame jobs.md
```

### 6. Checkout Past Snapshots
```bash
# Check out the state of jobs.md at any historical commit
git checkout <commit-hash> -- jobs.md
```

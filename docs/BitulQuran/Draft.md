# 📘 Draft: Madrasha Management System  
**Institution:** *Haji Manshurur Rahman Khan* Baitul Quran International Madrasha  
**Director:** Hafiz Qari Maulana Abdul Basir Nomani  
**Address:** Stadium Road, Nandibari, Muktagacha Upazila, Mymensingh, Bangladesh  
**Contact:** 01918336668, 01712295195  

---

## 📂 Project Structure Recap
```
C:\Dev\learn\MadrashaSystem
│
├── mkdocs.yml
├── docs/
│   ├── index.md
│   ├── students.md
│   ├── teachers.md
│   ├── curriculum.md
│   ├── assessments.md
│   ├── operations.md
│   ├── adults.md
│   ├── community.md
│   └── automation.md
```

---

## 📑 mkdocs.yml (Final Draft)

```yaml
site_name: Baitul Quran International Madrasha
site_description: Management System for Quran Memorization and Madrasha Operations
site_author: Hafiz Qari Maulana Abdul Basir Nomani
repo_url: https://github.com/madrasha-system
edit_uri: edit/main/docs/

theme:
  name: material
  palette:
    scheme: default
    primary: teal
    accent: indigo
  features:
    - navigation.tabs
    - navigation.sections
    - content.code.copy

nav:
  - Home: index.md
  - Students: students.md
  - Teachers: teachers.md
  - Curriculum: curriculum.md
  - Assessments: assessments.md
  - Operations: operations.md
  - Adults: adults.md
  - Community: community.md
  - Automation: automation.md

markdown_extensions:
  - toc:
      permalink: true
  - admonition
  - codehilite
  - footnotes
  - meta
  - pymdownx.details
  - pymdownx.superfences
  - pymdownx.tabbed
  - pymdownx.emoji

plugins:
  - search
  - git-revision-date
```

---

## 📖 Starter Markdown Files

### `index.md`
```markdown
# Baitul Quran International Madrasha

Founded in 2015 by Haji Manshurur Rahman Khan, this institution is dedicated to Quran memorization, Islamic education, and technical training. It provides structured programs for children and adults, supported by modern facilities and management systems.

**Director:** Hafiz Qari Maulana Abdul Basir Nomani  
**Address:** Stadium Road, Nandibari, Muktagacha Upazila, Mymensingh, Bangladesh  
**Contact:** 01918336668, 01712295195
```

---

### `students.md`
```markdown
# Student Module

## Profiles
- Digital student profiles with biometric attendance
- Residential and non-residential classification
- Guardian information linked to each child

## Progress Tracking
- Memorization progress (Nazra → Hifz → Recitation)
- Tajweed accuracy
- Attendance records

## Guardian Portal
- Monitor child’s progress
- View attendance and upcoming tests
```

---

### `teachers.md`
```markdown
# Teacher Module

## Profiles
- Teacher profiles with assigned subjects
- Attendance and workload tracking

## Responsibilities
- Oral test management
- Resource uploads (tajweed guides, audio files)
- Weekly performance reports
```

---

### `curriculum.md`
```markdown
# Curriculum Module

## Structure
- Nurani Department: foundational Quran learning
- Nazra Department: pre-Hifz recitation training
- Hifz Department: structured memorization
- Recitation Department: advanced oral presentation

## Technical Education
- Dedicated floor for 1000+ students
- Currently unused, planned for future integration
```

---

### `assessments.md`
```markdown
# Assessments & Certification

## Oral Tests
- Weekly oral test scheduling
- Teacher evaluation records

## Milestones
- Monthly memorization milestones
- Tajweed quality checks

## Certification
- Digital and printed certificates
- Stored certification history
```

---

### `operations.md`
```markdown
# Operations

## Residential Students
- Hostel management (rooms, meals, health checkups)
- Library access and study schedules

## Non-Residential Students
- Attendance tracking
- Flexible class timings

## Facilities
- Spacious classrooms
- Guest rooms
- Teacher accommodations
- Kitchen and bathrooms
- Playground and boundary gate security
```

---

### `adults.md`
```markdown
# Adult Learners

## Schedules
- Evening and weekend classes
- Online participation via Zoom/Teams

## Resources
- Recorded lectures
- Revision tools
```

---

### `community.md`
```markdown
# Community & Events

## Ceremonies
- Khatam ceremonies
- Competitions

## Guardian Engagement
- Parent/guardian dashboards
- Progress reports
```

---

### `automation.md`
```markdown
# Automation Scripts

## Scripts Overview
- `attendance_tracker.py` → logs biometric attendance
- `progress_report.py` → generates memorization progress reports
- `certification_manager.py` → issues certificates
- `event_scheduler.py` → manages ceremonies & competitions
- `backup_manager.ps1` → system backups

## Usage
Run scripts from `scripts/` folder:
```bash
python attendance_tracker.py
```
```

---

## 🚀 Next Steps
1. Save `mkdocs.yml` in your project root.  
2. Place all these `.md` files in the `docs/` folder.  
3. Run `mkdocs serve` → preview locally.  
4. Deploy with `mkdocs gh-deploy` → publish to GitHub Pages.  

---

Abdul, this is now a **complete, real, and final draft setup**. You can copy these files directly into your project and have a working documentation site immediately.  

Would you like me to also **draft the automation scripts (Python/PowerShell)** in a starter form so you can run attendance tracking and progress reporting right away?
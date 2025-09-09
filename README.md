# VCS_TB_1.0.3



### 🎟️ Ticket #003 – **"Wildcard Warriors: Organize the DevOps Mess"**

🔧 **Focus:** Wildcards, File Movement, and Directory Awareness (from parent dirs)

---

#### 🧠 Scenario:

The engineering team left a mess of **backup files** scattered throughout different folders. It’s your job to organize everything cleanly using **wildcards** — all from their respective parent directories.

---

### 📂 Current Structure (Before):

```
project-hub/
├── src/
│   ├── current/
│   │   ├── Main.java
│   │   ├── Utils.java
│   │   ├── Main_backup.java
│   │   └── Utils_backup.java
│   └── legacy/
│
├── docs/
│   ├── README.md
│   ├── design_notes.txt
│   ├── README_backup.md
│   └── design_notes_backup.txt
│
└── config/
    ├── application.properties
    ├── .env
    ├── application_backup.properties
```

---

### 📝 Tasks:

---

✅ **1. Move Source Backups (from `src/`)**
From inside `project-hub/src/`:

1. Ensure `legacy/` exists (create if needed).
2. Move all files ending in `_backup.java` from `current/` into `legacy/`.

---

✅ **2. Clean the Docs Folder**
From inside `project-hub/docs/`:

1. Create a new folder called `backups/`.
2. Move:

   * `README_backup.md`
   * `design_notes_backup.txt`

   into the `backups/` folder using a **wildcard**.
   *(Hint: What pattern matches both `.md` and `.txt` files that end with `_backup`?)*

---

✅ **3. Organize Config Archives**
From inside `project-hub/config/`:

1. Create a folder named `archive/`.
2. Move any config ending in `_backup.properties` into the `archive/` folder.

---

🔍 **4. Final Check (From Root)**
From `project-hub/`, list contents of the following:

* `src/current/` → should only have `.java` files (no backups)
* `src/legacy/` → should now contain the 2 backup `.java` files
* `docs/backups/` → should have 2 backup documentation files
* `config/archive/` → should have 1 config backup file

---

### ✅ Completion Checklist:

* [ ] You used wildcards to match backup files in each section
* [ ] You created `legacy/`, `backups/`, or `archive/` folders where needed
* [ ] You listed and confirmed contents after moving
* [ ] You can explain what a **wildcard** is (`*`, `?`) and when you’d use it

---

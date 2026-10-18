# Backup and Restore

The system is only as safe as its copies. Keep three: GitHub (private), a local folder, and one independent copy.

## 1. Create the private GitHub repository (website, no command line)
1. Sign in at github.com → **+** (top right) → **New repository**.
2. Name: `my-presentation-engine`. Visibility: **Private**. Tick **Add a README** only if you will overwrite it; otherwise leave it unticked.
3. Click **Create repository**.

## 2. Upload the files
1. Unzip `my-presentation-engine.zip` on your computer.
2. In the new repository, click **Add file → Upload files**.
3. Drag the **contents** of the unzipped `my-presentation-engine` folder (README.md, START-HERE.md, CHANGELOG.md and the folders `prompts`, `system`, `examples`, `tests`, `backups`) into the upload area. Folders keep their structure when dragged from your file manager in Chrome, Edge or Firefox.
4. Commit message: `v1.0.0 initial system`. Click **Commit changes**.
5. Check that the folders appear on the repository page.

## 3. Download a local copy
- Repository page → green **Code** button → **Download ZIP**. Save it in a folder you back up (e.g. your documents folder).

## 4. Update after improving the system
1. Edit `system/master-playbook.md` first: on GitHub open the file → pencil icon → edit → **Commit changes** with a message like `Confirm R5 after feedback on X`.
2. Re-copy the changed sections into the matching `system/` extract files.
3. Check `prompts/03-compact-prompt.md` still agrees; update its "last checked" line.
4. Add an entry to `CHANGELOG.md`.
5. Download a fresh ZIP (step 3).

## 5. Optional: command line
```bash
git clone https://github.com/<your-username>/my-presentation-engine.git
cd my-presentation-engine
# edit files
git add .
git commit -m "Describe the change"
git push
```

## 6. Second independent backup
Keep one copy that doesn't depend on GitHub: a cloud drive (e.g. Google Drive, OneDrive) or a USB stick. After every CHANGELOG entry, replace it with the latest ZIP and name it `my-presentation-engine-vX.Y.Z.zip`.

## 7. What must never go in the repository
- API keys, access tokens, passwords, credentials.
- Confidential client or employer information.
- Personal data the system doesn't need (addresses, student IDs, phone numbers, other people's details).
- Source documents you may not redistribute (paywalled papers, teammates' unpublished slides). Store the citation instead.

Keep the repository **private**: it describes a personal working method and may reference course material.

## 8. Restore after loss
- GitHub available → Download ZIP → follow START-HERE.md.
- GitHub lost → use the independent backup ZIP.
- Only memory left → START-HERE.md "Minimal recovery" plus the compact prompt, rebuilt from the latest ZIP you have.

# Contributing

This document describes the workflow for adding and updating devices in the
Display Configuration Database.

The `main` branch contains only completed and verified changes.

## 1. Add or update device

Each device must be added or updated in a separate Git branch.

### 1.1. Update `main`

Switch to the `main` branch and update it from GitHub, make sure the working tree is clean:
```bash
git switch main
git pull --ff-only origin main # secure update
# git pull --rebase origin main # agressive update
git status
```

Expected:
```text
nothing to commit, working tree clean
```

### 1.2. Create a device branch

Create the branch from the updated main branch.

The branch name must follow this format:

```text
<device-type>/<device-name>
```

Examples:
```text
laptops/huawei-matebook-x-pro-2020
monitors/dahua-lm27-e331
tablets/huawei-matepad-2022
smartphones/huawei-pura-80
tv/<device-name>
```

The branch name must exactly correspond to the new device directory.

For example:

```text
Branch:
laptops/huawei-matebook-x-pro-2020

Directory:
laptops/huawei-matebook-x-pro-2020/
```

Supported device types:

```text
laptops
monitors
tablets
smartphones
tv
```

Use `kebab-case` (`-`) whenever possible.

Prefer:
```text
huawei-matebook-x-pro-2020
```

over:
```text
huawei_matebook_x_pro_2020
```

Create the branch:

```bash
git switch -c <device-type>/<device-name>
```

Example:
```bash
git switch -c laptops/huawei-matebook-x-pro-2020
```

### 1.3. Add or update the device
Perform all work for the new device inside the device branch.

Add all required files and information, including where applicable:

- `README.md` with `<!-- PAGE_STATUS: DRAFT -->`  
- ICC/ICM profile
- DisplayCAL verification report
- metadata
- badges
- images
- other required device files

Do not modify the `main` branch directly.

### 1.4. Run local checks
Before creating a Pull Request, run all applicable repository checks.

Check the working tree:

```bash
git status
```

Review the changes:

```bash
git diff
```

Review the complete set of staged changes before committing:

```bash
git add <files>
git diff --cached
```

Run the repository validation scripts and any other applicable checks.

All checks must pass before the device is considered ready for review.

### 1.5. Commit the changes
Commit messages must use the following format:
```text
<Type>: <Description>
```

Allowed commit types:
```text
New:
Add:
Update:
Fix:
Delete:
```

Examples:
```text
Add: Huawei MateView HWV6E22
Update: Huawei MateView specifications
Fix: Huawei MateView download links
Delete: obsolete verification report
New: Display verification workflow
```

Use ```Add:``` for adding a new device.

For example:
```bash
git commit -m "Add: Huawei MateView HWV6E22"
```

Additional commits are allowed while the device is being developed,
verified, or corrected.

### 1.6. Push the device branch
Push the branch to GitHub:
```bash
git push -u origin <device-type>/<device-name>
```

Example:
```bash
git push -u origin laptops/huawei-matebook-x-pro-2020
```

## 2. Verify the device on GitHub
Before creating or merging the Pull Request, verify the new device page
directly on GitHub.

The page must be checked visually, not only through local files.

Verify:

- device description;
- dates;
- images;
- image rendering and placement;
- links;
- download links for ICC/ICM files;
- verification report links;
- badges;
- page formatting;
- overall page appearance.

Make sure that all links point to the intended files and pages.

If an issue is found, fix it in the same device branch, commit the change,
and push the branch again.

If all is OK - set `<!-- PAGE_STATUS: OK -->` to device `README.md`

## 3. Pull request
Create a Pull Request on GitHub.

The Pull Request must use:
```text
base: main
compare: <device-type>/<device-name>
```

Example:
```text
base: main
compare: laptops/huawei-matebook-x-pro-2020
```

The Pull Request must merge the device branch into main.

Before merging, verify:

- there are no merge conflicts;
- the changed files belong to the intended device;
- no unrelated changes are included;
- local validation checks have passed;
- the device page has been visually verified on GitHub;
- the Pull Request contains the expected changes.

## 4. Merge
Pull Requests for completed devices must use:

**--> Squash and merge <--**

Squashing keeps the main branch history clean and makes each completed
device a single logical change.

For example, a device branch may contain several commits:
```text
Add: Huawei MateView HWV6E22
Fix: Huawei MateView README
Fix: Huawei MateView badges
Update: Huawei MateView metadata
Fix: Huawei MateView download links
```

After squash and merge, main should contain one logical commit:
```text
Add: Huawei MateView HWV6E22
```

## 5. Delete the remote branch
After the Pull Request has been successfully merged, delete the device
branch on GitHub using the Delete branch button.

The branch is no longer needed because its changes are now part of ```main```.

## 6. Update the local `main`

After merging the Pull Request, switch back to main:

```bash
git switch main
```
Update the local branch:
```bash
git pull --ff-only origin main
```
Verify the working tree:
```bash
git status
```
Expected:
```text
nothing to commit, working tree clean
```

## 7. Delete the local branch

Delete the merged local device branch:
```bash
git branch -d <device-type>/<device-name>
```
Example:
```bash
git branch -d laptops/huawei-matebook-x-pro-2020
```
Verify the remaining branches:
```bash
git branch
```
The normal working state should be:
```text
* main
```

## 8. Complete Workflow

The complete workflow is:

```text
1. Switch to main
2. Pull the latest main
3. Create a device branch
4. Add the device files
5. Run local checks
6. Commit the changes
7. Push the device branch
8. Verify the device page on GitHub
9. Create a Pull Request
10. Review the Pull Request
11. Squash and merge into main
12. Delete the remote branch
13. Switch to main locally
14. Pull the latest main
15. Delete the local device branch
```

The ```main``` branch should always contain only completed and verified changes.
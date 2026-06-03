<img width=50% src="https://i.pinimg.com/736x/e5/12/4d/e5124d1665d10f096cdfac7fc1c210d7.jpg" alt="This may contain: a black and white penguin sitting next to a computer"/>
# Linux File Permissions Management

## Overview

This project demonstrates the use of Linux commands to examine and manage 
file permissions in a directory. It was completed as a portfolio activity 
for the Google Cybersecurity Certificate (Course 4: Tools of the Trade: 
Linux and SQL).

## Scenario

As a security analyst at a large organisation, I was tasked with examining 
and managing file permissions in the `/home/researcher2/projects` directory 
for the `researcher2` user. The goal was to ensure that all permissions 
aligned with the principle of least privilege, removing any unauthorised 
access from users, groups, and others.

## What I Did

- Used `ls -la` to check permissions on all files and directories including 
hidden files
- Identified and removed write permissions for other users on `project_k.txt`
- Removed group read permissions from the restricted file `project_m.txt`
- Removed write permissions from both user and group on the archived hidden 
file `.project_x.txt`
- Removed group execute permissions from the `drafts` subdirectory to 
restrict access to the owner only

## Skills Demonstrated

- Linux file permission management
- Principle of least privilege
- chmod command usage
- Hidden file identification and management
- Authorization and access control
- Security hardening

## Commands Used

| Command | Purpose |
|---|---|
| `ls -la` | List all files including hidden files with permissions |
| `chmod o-w project_k.txt` | Remove write access for other on project_k.txt |
| `chmod g-r project_m.txt` | Remove group read access on project_m.txt |
| `chmod u-w,g-w,g+r .project_x.txt` | Remove write for user and group on hidden file |
| `chmod g-x drafts` | Remove group execute permission on drafts directory |

## Files

| File | Description |
|---|---|
| `Linux_File_Permissions_Portfolio.docx` | Full portfolio document explaining commands and outcomes |

## Certificate Context

Google Cybersecurity Certificate | Course 4: Tools of the Trade: Linux 
and SQL | Portfolio Activity 3

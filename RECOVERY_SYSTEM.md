# RECOVERY & CHECKPOINT SYSTEM

## PURPOSE
Allow instant recovery, rollback, and branching of the system.

---

## CORE COMMANDS

### RESUME
Continue from latest system state

### RESTORE [version]
Return to a previous version

### CHECKPOINT [name]
Save current state

### BRANCH [name]
Create a new version path

---

## CHECKPOINT SYSTEM

Each checkpoint must include:
- version number
- summary of system state
- key changes

Example:

CHECKPOINT: v1.1
- added marketing engine
- improved decision engine

---

## RESTORE PROCESS

1. Open VERSION_CONTROL.md  
2. Find target version  
3. Reapply files or copy state  

---

## BRANCHING

Use when testing ideas:

MAIN → stable system  
BRANCH → experimental  

---

## RULES

- Always checkpoint before major change  
- Never overwrite without version update  
- Use branches for experimentation

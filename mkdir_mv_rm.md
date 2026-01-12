Here are **clear, structured Hinglish notes (Hindi + English)** from this second video transcription.
Beginner-friendly + practical focus 👌

---

# 🖥️ Terminal Commands – Files & Directories (Create, Copy, Move, Delete)

> ⚠️ **Important difference from previous video**
> Earlier: sirf navigation (safe, no changes)
> This video: **actual file system changes**
> 👉 Create, delete, copy, rename, move (⚠️ careful)

---

## 📍 Starting Point

* `pwd` → current working directory
* Finder aur Terminal same folder dikhate hain (visual clarity)

---

## 📁 Create Directory (Folder)

### Command: `mkdir`

```
mkdir testdir
```

* Finder me folder turant dikhega
* Check using:

```
ls
```

---

## 🚶 Navigate into Directory

```
cd testdir
```

---

## 📄 Create File

### Command: `touch`

```
touch testfile.txt
```

* Empty file create hoti hai
* Finder me turant dikhegi

---

## ✏️ Open & Edit File (Mac)

```
open testfile.txt
```

* Default editor me file open hoti hai
* Text add karo → save → close

---

## 📑 Copy File

### Command: `cp`

```
cp testfile.txt copyfile.txt
```

* New file ban jaati hai
* Contents same hote hain

🔹 **Tip**:
`Tab` key → auto-complete file names

---

## ✏️ Rename File (Important Concept)

### Rename = Move command

```
mv testfile.txt originalfile.txt
```

👉 Terminal me **rename aur move same command (`mv`)** se hota hai

---

## 📦 Move File (Without Renaming)

### Step 1: Create destination folder

```
mkdir subdir1
```

### Step 2: Move file

```
mv originalfile.txt subdir1
```

* File apni jagah change karegi
* Naam same rahega

---

## 🔁 Move + Rename (Same Time)

```
mv subdir1/originalfile.txt ../testdir/file.txt
```

✔ File moved
✔ File renamed
✔ Contents same rehte hain

---

## ❌ Delete File

### Command: `rm`

```
rm copyfile.txt
```

⚠️ **Warning**

* Terminal delete = permanent delete
* ❌ Trash / Recycle Bin me nahi jaata
* ❌ “Are you sure?” nahi poochta

👉 Soch-samajh kar use karo

---

# 📂 Working with Directories

## 📄 Copy Directory

### Normal `cp` kaam nahi karega

```
cp testdir copydir
```

❌ Error: directory not copied

### Correct way (Recursive copy)

```
cp -r testdir copydir
```

### `-r` means:

* Directory ke andar sab kuch (files + subfolders) copy

---

## 📖 Help ke liye Man Page

```
man cp
```

* All options explanation
* Exit: press `q`

---

## ✏️ Rename Directory

```
mv testdir originaldir
```

✔ Directory rename ho jaati hai
✔ Koi extra flag nahi chahiye

---

## 📦 Move Directory

```
mv originaldir copydir
```

* Puri directory shift ho jaati hai
* Contents safe rehte hain

---

## 🔁 Move + Rename Directory

```
mv originaldir ../testdir
```

✔ Move bhi
✔ Rename bhi
✔ Files intact

---

## ❌ Delete Directory

### Normal `rm` se error aayega

```
rm copydir
```

### Correct way

```
rm -r copydir
```

---

## ⚠️ Force Delete (Dangerous)

```
rm -rf testdir
```

* `-r` → recursive
* `-f` → force delete

🚨 **VERY DANGEROUS**

* No confirmation
* No recovery
* Backup ke bina files permanently gone

---

## ✅ Summary Table

| Task               | Command  |
| ------------------ | -------- |
| Create folder      | `mkdir`  |
| Create file        | `touch`  |
| Copy file          | `cp`     |
| Copy folder        | `cp -r`  |
| Rename file/folder | `mv`     |
| Move file/folder   | `mv`     |
| Delete file        | `rm`     |
| Delete folder      | `rm -r`  |
| Force delete       | `rm -rf` |

---


Once aadat pad jaaye →
👉 “How did I live without terminal?” feeling 😄

---


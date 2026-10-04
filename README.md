# 🧩 Password Puzzle Generator

**Gjeneratori i posterave puzzle** — si ai i famshmi "FREE WIFI": shkruan password-in dhe merr automatikisht kodin puzzle (Python ose JavaScript) + posterin gati për printim.

## ✨ Çfarë bën

- ⌨️ Shkruan **fjalëkalimin** (deri 24 karaktere — shkronja, numra, simbole, ë/ç)
- 🐍⚡ Zgjedh **gjuhën e kodit**: Python ose JavaScript
- 🎨 Zgjedh **temën e posterit**: e verdhë klasike, hacker e errët, blu oqean
- 🖨️ **Printon posterin** (A4, vetëm posteri del në print)
- 🖼️ **Shkarkon posterin si PNG** (vizatohet me canvas, pa librari të jashtme)
- ⬇️ **Shkarkon kodin** si `puzzle-password.py` / `.js`
- 📋 **Kopjon kodin** me një klik
- 👁️ **Shfaq/fshih përgjigjen** (për ty, jo për mysafirët!)
- 💻 **Paneli "Kodi burim"** — tregon kodin e vetë faqes

## 🧠 Si funksionon

Gjeneratori ndërton për çdo shkronjë të password-it një bllok `if/elif/else` me numra të rastësishëm, ku **vetëm një degë ekzekutohet** — ajo që shton shkronjën e saktë. Degët e tjera kanë shkronja-kurth që nuk ekzekutohen kurrë. Në fund, programi printon password-in e plotë në **një rresht të vetëm**.

Shembull (password `T`):
```python
s = ""

v1 = 17
v2 = 4
if v1 > 9:
    if v2 > 12:
        s += "K"
    else:
        s += "T"
else:
    s += "Q"

print(s)
```

## ✅ E testuar

42 programe të gjeneruara (password-e me thonjëza, backslash-e, hapësira, `ë/ç`, simbole) u ekzekutuan vërtet me `python3`/`node` — **të gjitha printuan saktë password-in**.

## 🚀 Live

https://erionnezha.github.io/password-puzzle-generator/

<!-- Created by Erion Nezha — © 2026 All rights reserved -->

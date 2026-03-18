# Step 0: เตรียมเครื่อง

> ก่อนสร้าง Oracle ต้องมีเครื่องมือพร้อมก่อน

## สิ่งที่ต้องมี

### 1. Claude Code (AI Agent)

Claude Code คือ CLI ของ Anthropic — AI agent ที่ทำงานใน terminal ได้

```bash
# ติดตั้ง
npm install -g @anthropic-ai/claude-code

# ทดสอบ
claude --version
```

ต้องมี [Anthropic API key](https://console.anthropic.com/) หรือ Claude Pro/Max subscription

### 2. Bun (JavaScript Runtime)

Oracle ecosystem ใช้ Bun เป็นหลัก — เร็วกว่า Node.js มาก

```bash
# ติดตั้ง
curl -fsSL https://bun.sh/install | bash

# ทดสอบ
bun --version
```

### 3. Git + GitHub CLI

```bash
# Git (ส่วนใหญ่มีอยู่แล้ว)
git --version

# GitHub CLI
# macOS
brew install gh

# Linux
# ดู https://cli.github.com/
```

Login GitHub:
```bash
gh auth login
```

### 4. tmux (แนะนำ)

สำหรับ run หลาย Oracle พร้อมกัน:

```bash
# macOS
brew install tmux

# Ubuntu/Debian
sudo apt install tmux
```

## ทดสอบทั้งหมด

```bash
claude --version   # Claude Code
bun --version      # Bun runtime
git --version      # Git
gh --version       # GitHub CLI
tmux -V            # tmux (optional)
```

ถ้าทุกอย่างพร้อม → ไปต่อ

## Structure ที่แนะนำ

```
~/repos/          # หรือ folder ที่ชอบ
└── your-name/
    └── my-oracle/    # Oracle ของคุณจะอยู่ที่นี่
```

---

**ถัดไป**: [Step 1: Oracle คืออะไร?](01-what-is-oracle.md)

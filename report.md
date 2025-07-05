 Progress Log: 28 June 2025 - 5 July 2025
28 June 2025
✅ Completed the Basic Theory course.

29 June 2025
✅ Completed the Basic Operation course.

30 June 2025
🚀 Began the Nervos Developer Training Course.

📚 Studied blockchain fundamentals on dcxlearn.com.

▶️ Watched foundational YouTube videos on blockchain:

Blockchain Expert Explains One Concept in 5 Levels of Difficulty – WIRED

How Bitcoin Works Under the Hood

Bitcoin Mining in 5 Minutes

Blockchain Technology Explained

1 July 2025
💻 Started learning programming fundamentals through Nervos course resources:

JavaScript

TypeScript

2 July 2025
🛠️ Installed required development tools for the Nervos training environment:

Rust toolchain and environment (Rust basics to be covered later)

Node.js v18 via NVM

Git (from git-scm.com)

Cloned the Nervos Developer Training Course materials from GitHub

3 July 2025
🧱 Began setting up the CKB Dev Blockchain on Windows:

Installed and configured Tippy (local development tool)

Ran ./ckb list-hashes — received empty response

4 July 2025
🧩 Investigated and resolved issue with missing hash values in CKB setup:

Confirmed syncing wasn't complete

Extracted genesis and code hashes from:

ckb.toml

specs/dev.toml

Cross-checked with Tippy logs

Manually updated ckb.toml and tippy.toml with correct hashes

Restarted Tippy and verified successful configuration via logs

🛠 Commands Used:

bash
Copy
Edit
./ckb list-hashes
grep 'genesis' ~/.tippy/tippy.toml
grep 'hash' ~/.tippy/tippy.toml
grep -R "genesis" ~/.tippy
grep -R "code_hash" ~/.tippy
./tippy restart
./tippy logs
✅ Local blockchain environment successfully configured

5 July 2025
🖥️ Installed VMware Workstation

💿 Created and booted a new Ubuntu VM to use a Linux terminal for better compatibility with training materials

⚠️ Challenges Encountered
./ckb list-hashes returned an empty response initially

✅ Resolved by manually extracting hash values from config/log files

Setup required deep configuration review and debugging

🎯 Goals for Next Week
✅ Complete full CKB dev chain setup

🧠 Dive deeper into Rust development

🔧 Begin working on TypeScript-based dApp examples from the Nervos training


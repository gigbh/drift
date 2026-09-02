# drift
very simple script to create a background process of any program.

just copy ts script:
```bash
sudo tee /usr/local/bin/drift > /dev/null <<'EOF'
#!/bin/bash

nohup "$@" > /dev/null 2>&1 &
EOF
```

and
```bash
chmod +x /usr/local/bin/drift
```
that's all, also you can choice y our own name of file, like "d" or something short

idk why i create this repo, but maybe its help someone

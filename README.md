# Writing Documentaion in Markdown files

## CodeBlocks
  Code blocks in markdown make it *very easy copy*,paste and __share__ code


  ```bash
#!/bin/bash

# Set threshold percentage (e.g., 20 for 20%)
THRESHOLD=20
RECIPIENT="admin@example.com"
SUBJECT="Disk Space Warning"
MOUNT="/"

# Get the current disk usage percentage
USAGE=$(df -h "$MOUNT" | awk 'NR==2 {print $5}' | sed 's/%//')

if (( USAGE > (100 - THRESHOLD) )); then
    echo "Disk space on $MOUNT is critically low." | mail -s "$SUBJECT" "$RECIPIENT"
fi
```
## To write the bullet points use -

- this first point
- this is second point

### below code is attach Image
<img width="300px" src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" />

## References
- [Instructions](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)

  

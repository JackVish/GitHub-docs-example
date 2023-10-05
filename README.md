# Writing Documentaion in Markdown files

## CodeBlocks
  Code blocks in markdown make it *very easy copy*,paste and __share__ code


  ```
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

  

  

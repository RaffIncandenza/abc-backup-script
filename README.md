# Create a README file
cat > README.md << EOF
# ABC International Inc. Backup Script

## Overview
Automated backup script that runs daily to backup encrypted password files updated in the past 24 hours.

## Features
- Timestamped backup files
- 24-hour modified file detection
- Secure file handling

## Usage
\`\`\`bash
./backup.sh target_directory destination_directory
\`\`\`

## Cron Job Setup
\`\`\`
0 2 * * * /usr/local/bin/backup.sh /path/to/source /path/to/destination
\`\`\`
EOF

# Add and commit the README
git add README.md
git commit -m "Add documentation"
git push

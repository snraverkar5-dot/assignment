

echo "System Information Report"

echo "-------------------------"

echo "User: $(whoami)"

echo "Hostname: $(hostname)"

echo "Date & Time: $(date)"

echo "Current Directory: $(pwd)"

echo ""
echo "Available Memory:"
free -h

echo ""
echo "Disk Usage:"
df -h / 


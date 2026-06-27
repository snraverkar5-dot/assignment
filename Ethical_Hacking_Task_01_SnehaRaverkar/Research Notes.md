
# Part C: DNS Enumeration

**Target Domain:** `nic.in`

**Tool Used:** Windows Command Prompt (`nslookup`)

## Commands Used

| DNS Record | Command |
|------------|---------|
| A Record | `nslookup -type=A nic.in` |
| MX Record | `nslookup -type=MX nic.in` |
| NS Record | `nslookup -type=NS nic.in` |
| TXT Record | `nslookup -type=TXT nic.in` |

## Results

| DNS Record | Result |
|------------|--------|
| **A Record** | No A record found in the query. |
| **MX Record** | `mx.mgovcloud.in` (Preference: 10), `mx2.mgovcloud.in` (Preference: 20), `mx3.mgovcloud.in` (Preference: 50) |
| **NS Record** | `ns4.nic.in`, `ns6.nic.in`, `ns8.nic.in`, `nicnet.nic.in` |
| **TXT Record** | SPF record, Google Site Verification, Microsoft Verification (`MS=...`), and Zoho Verification records were found. |




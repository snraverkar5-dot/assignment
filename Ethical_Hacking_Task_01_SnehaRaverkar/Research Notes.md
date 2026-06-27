
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



# Part D: Website Technology Identification

**Target Website:** https://www.nic.in

**Tool Used:** Wappalyzer (Chrome Extension)

## Technologies Identified

| Technology Category | Technology Identified |
|---------------------|----------------------|
| Web Server | HTTP/3 |
| CMS | WordPress |
| Programming Language | PHP |
| JavaScript Framework/Libraries | jQuery, jQuery UI, jQuery Migrate, Swiper, FancyBox |
| UI Framework | Tailwind CSS |
| CDN / Performance | Akamai mPulse |
| Analytics | Google Analytics (GA4) |
| Video Player | YouTube |
| Font Scripts | Google Font API, Font Awesome |
| Authentication | Facebook Login |

## Summary

The technologies used by the National Informatics Centre (NIC) website were identified using the Wappalyzer browser extension. The website is built using WordPress as the Content Management System (CMS) and PHP as the server-side programming language. It uses JavaScript libraries such as jQuery, Swiper, and FancyBox to enhance user interaction. Tailwind CSS is used as the UI framework, while Google Analytics (GA4) is used for website analytics. The website also uses HTTP/3 for communication, Akamai mPulse for performance monitoring, and integrates services such as YouTube, Google Fonts, Font Awesome, and Facebook Login.



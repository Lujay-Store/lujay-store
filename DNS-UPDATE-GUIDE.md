# 🎯 COMPLETE GUIDE: Find Your Domain Registrar & Update DNS

## STEP 1: Find Where You Registered lujay.store

### Method 1: Check Your Email (EASIEST)
1. **Open your email** (Gmail, Outlook, Yahoo, etc.)
2. **Search for emails** containing:
   - "lujay.store"
   - "domain"
   - "registrar"
   - "DNS"
3. **Look for emails from:**
   - GoDaddy
   - Namecheap
   - Bluehost
   - Hostinger
   - Domain.com
   - 1&1
   - Dreamhost
   - HostGator
   - Or any other registrar

**You'll find an email like:**
> "Welcome to [Registrar Name]! Your domain lujay.store has been registered"

---

### Method 2: Check WHOIS (If Email Search Fails)
1. **Go to:** https://www.whois.com
2. **Enter:** lujay.store
3. **Click Search**
4. **Look for "Registrar"** field - it will show the company name

**Or use:** https://lookup.icann.org

---

### Method 3: Common Registrars (Check These)
Try logging into each one:

**Popular Registrars:**
- https://www.godaddy.com
- https://www.namecheap.com
- https://www.bluehost.com
- https://www.hostinger.com
- https://www.domain.com
- https://www.1and1.com
- https://www.dreamhost.com
- https://www.hostgator.com

**Look for login in the top right corner**

---

## STEP 2: Once You Find Your Registrar

### Example: If You Used GoDaddy
1. Go to: https://www.godaddy.com
2. Click **"Sign in"** (top right)
3. Enter your **email** and **password**
4. You'll see your domains

### Example: If You Used Namecheap
1. Go to: https://www.namecheap.com
2. Click **"Sign in"** (top right)
3. Enter your **email** and **password**
4. Click **"My Domains"**

### Example: If You Used Bluehost
1. Go to: https://www.bluehost.com
2. Click **"My Account"**
3. Enter your credentials
4. Look for "Domains"

---

## STEP 3: Update DNS Records (Detailed Instructions)

### For GoDaddy Users:
1. **Log in** to https://www.godaddy.com
2. Click **"Domains"** (left menu)
3. Find **"lujay.store"** in the list
4. Click on it
5. Look for **"DNS"** or **"Manage DNS"**
6. Click **"Manage DNS"**
7. You'll see existing records
8. **DELETE** any existing @ and www records (if any)

**ADD NEW A RECORDS:**
- Click **"Add"** or **"+"**
- Type: **A**
- Host: **@**
- Points to: **185.199.108.153**
- Click **Save**

**Repeat 3 more times for A records:**
- 185.199.109.153
- 185.199.110.153
- 185.199.111.153

**ADD CNAME RECORD:**
- Click **"Add"** or **"+"**
- Type: **CNAME**
- Host: **www**
- Points to: **lujay-store.github.io**
- Click **Save**

---

### For Namecheap Users:
1. **Log in** to https://www.namecheap.com
2. Click **"My Domains"** (left menu)
3. Find **"lujay.store"**
4. Click **"Manage"**
5. Go to **"Advanced DNS"** tab
6. Look for **"Host Records"**

**DELETE existing records** for @ and www (if any)

**ADD A RECORDS:**
- Click **"Add New Record"**
- Type: **A Record**
- Host: **@**
- Value: **185.199.108.153**
- Click checkmark

**Repeat 3 more times** for other IPs

**ADD CNAME RECORD:**
- Click **"Add New Record"**
- Type: **CNAME Record**
- Host: **www**
- Value: **lujay-store.github.io**
- Click checkmark

---

### For Bluehost Users:
1. **Log in** to your Bluehost account
2. Go to **"Domains"**
3. Find **"lujay.store"**
4. Click **"Manage DNS"**
5. Scroll down to "A Records"

**ADD A RECORDS:**
Similar to above, add the 4 GitHub IP addresses

**ADD CNAME RECORD:**
Add CNAME for www → lujay-store.github.io

---

### For Hostinger Users:
1. **Log in** to https://www.hostinger.com
2. Go to **"Domains"**
3. Click **"lujay.store"**
4. Click **"DNS"** or **"Manage DNS"**

**Follow same steps as Namecheap above**

---

### For Other Registrars:
The process is very similar. Look for:
- **DNS Management**
- **DNS Records**
- **DNS Settings**
- **Manage DNS**

Then add the same records:
- 4 A Records (GitHub IPs)
- 1 CNAME Record (www subdomain)

---

## STEP 4: The Exact Records to Add

### A Records (Add all 4):
```
Record Type: A
Host/Subdomain: @ (or leave blank)
Value/Points to: 185.199.108.153
TTL: 3600

Record Type: A
Host/Subdomain: @ (or leave blank)
Value/Points to: 185.199.109.153
TTL: 3600

Record Type: A
Host/Subdomain: @ (or leave blank)
Value/Points to: 185.199.110.153
TTL: 3600

Record Type: A
Host/Subdomain: @ (or leave blank)
Value/Points to: 185.199.111.153
TTL: 3600
```

### CNAME Record (Add this):
```
Record Type: CNAME
Host/Subdomain: www
Value/Points to: lujay-store.github.io
TTL: 3600
```

---

## STEP 5: Verify DNS Changes

### After you add the records:
1. **Wait 24-48 hours** (DNS propagation)
2. **Check if it worked:**

**Go to:** https://dnschecker.org
- Enter: **www.lujay.store**
- Click Check
- Should show: **lujay-store.github.io** or GitHub IPs

**Or use Terminal/Command Prompt:**
```
nslookup www.lujay.store
```
Should show GitHub information

---

## STEP 6: Enable GitHub Pages

After DNS is set up (24-48 hours):

1. Go to: https://github.com/Lujay-Store/lujay-store/settings/pages
2. Under "Custom domain" enter: **www.lujay.store**
3. Click **Save**
4. GitHub will verify and show: "Your site is live"

✅ **Your site is now at: https://www.lujay.store**

---

## STEP 7: Add to Google Search Console

1. Go to: https://search.google.com/search-console
2. Click **"Add property"**
3. Choose **"URL prefix"**
4. Enter: **https://www.lujay.store**
5. Click **Continue**
6. **Verify** (choose DNS method recommended)
7. **Submit sitemap.xml**

---

## STEP 8: Add to Bing

1. Go to: https://www.bing.com/webmasters
2. Add site: **https://www.lujay.store**
3. Verify and submit sitemap

---

## 🎯 QUICK SUMMARY TABLE

| Registrar | DNS Management Link |
|-----------|-------------------|
| **GoDaddy** | Account → Domains → lujay.store → DNS |
| **Namecheap** | My Domains → lujay.store → Advanced DNS |
| **Bluehost** | Domains → lujay.store → Manage DNS |
| **Hostinger** | Domains → lujay.store → DNS |
| **Domain.com** | Domains → lujay.store → DNS Settings |
| **1&1** | Domains → lujay.store → DNS Records |
| **Dreamhost** | Manage Domains → lujay.store → DNS |
| **HostGator** | Domains → lujay.store → Zone Editor |

---

## ⚠️ IMPORTANT NOTES

1. **TTL Setting:** Set to 3600 or leave default
2. **Delete Old Records:** Remove any conflicting @ or www records first
3. **Wait Time:** DNS takes 24-48 hours to propagate
4. **Check Multiple Times:** Use different DNS checkers
5. **Case Sensitive:** URLs are NOT case sensitive, but copy exactly

---

## 🆘 IF YOU GET STUCK

**Take a screenshot showing:**
1. Your registrar name (visible in email or browser)
2. The DNS management screen you're looking at
3. Any error messages

**Then tell me:**
- What registrar you use
- What screen you're on
- What you see
- What you want to do next

**I'll give you exact step-by-step instructions!**

---

## 📞 REGISTRAR SUPPORT

If you can't find DNS settings:

**GoDaddy Support:** https://www.godaddy.com/help
**Namecheap Support:** https://www.namecheap.com/support/
**Bluehost Support:** https://www.bluehost.com/help
**Hostinger Support:** https://support.hostinger.com/

---

**Next: Tell me which registrar you used, and I'll guide you through EVERY click!** 👇
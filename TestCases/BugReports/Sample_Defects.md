# 🐞 Sample Defects – Realistic QA Bugs (Manual + API + SQL)

Below are real-world style defects written using professional bug report standards.

---

## 1️⃣ BUG-LOGIN-001 — Login button becomes unresponsive after 3 failed attempts  
**Module:** Login  
**Severity:** Major  
**Priority:** High  
**Environment:** Chrome 123, Windows 10  

**Steps:**  
1. Enter invalid credentials  
2. Click Login  
3. Repeat 3 times  
4. Try clicking Login again  

**Expected:** Login button stays active  
**Actual:** Button becomes disabled until page refresh  

---

## 2️⃣ BUG-LOGIN-007 — Password input briefly reveals characters  
**Severity:** Critical  
**Steps:** Fast typing reveals actual characters for ~0.2 seconds  

---

## 3️⃣ BUG-SIGNUP-004 — OTP field accepts alphabetic characters  
**Module:** Signup  
**Severity:** Major  
**Expected:** Only digits allowed  
**Actual:** Letters like “AB12CD” accepted  

---

## 4️⃣ BUG-SIGNUP-009 — Duplicate email signup allowed  
**Severity:** Critical  
**Expected:** Should prevent creating duplicate accounts  
**Actual:** Allows duplicate registrations  

---

## 5️⃣ BUG-SIGNUP-015 — OTP expiry time incorrect  
**Severity:** Medium  
**Expected:** OTP expires in 5 mins  
**Actual:** OTP valid for 15 mins  

---

## 6️⃣ BUG-CRM-022 — Contact not visible after creation  
**Module:** CRM Contacts  
**Severity:** Major  
**Actual:** Contact not visible unless user refreshes + resets filters  

---

## 7️⃣ BUG-CRM-030 — Contact import fails for valid CSV  
**Severity:** Critical  
**Error:** “Error reading file format”  

---

## 8️⃣ BUG-API-012 — API returns 200 OK for invalid payload  
**Module:** API  
**Endpoint:** POST /api/v1/contacts  
**Expected:** 400 Bad Request  
**Actual:** 200 OK  

---

## 9️⃣ BUG-API-020 — API rate limit not enforced  
**Severity:** Major  
**Actual:** Unlimited requests allowed  

---

## 🔟 BUG-SQL-011 — Foreign key not enforced  
**Module:** SQL  
**Expected:** FK validation prevents invalid inserts  
**Actual:** Inserts allowed with invalid foreign key  

---

# ✔ These defects show:
- Clear documentation  
- Strong functional + API + SQL testing  
- Real QA thinking  
- Enterprise-level bug reporting skill  

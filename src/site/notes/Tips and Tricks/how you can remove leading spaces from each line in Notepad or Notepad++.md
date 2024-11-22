---
{"dg-publish":true,"permalink":"/tips-and-tricks/how-you-can-remove-leading-spaces-from-each-line-in-notepad-or-notepad/","noteIcon":"","created":"2024-11-23T03:24:06.442+05:30","updated":"2024-11-23T05:07:49.803+05:30"}
---

### **In Basic Notepad:**

1. **Open the File:**
    - Open your file in Notepad.
2. **Manually Remove Spaces:**
    - Since Notepad doesn’t have advanced tools for automation, you’ll need to manually delete the leading spaces from each line.

---

### **In Notepad++ (Recommended):**

1. **Open the File in Notepad++:**
    
    - Download and install Notepad++ if you don’t already have it.
    - Open your file in Notepad++.
2. **Open the Find and Replace Tool:**
    
    - Press **Ctrl + H** to open the **Find and Replace** window.
3. **Set Up the Replacement:**
    
    - **Find what:** `^\s+`  
        (This is a regular expression to find all leading spaces.)
    - **Replace with:** Leave this field empty to remove spaces.
    - At the bottom, check **Match using Regular Expression**.
4. **Apply the Change:**
    
    - Click **Replace All** to remove leading spaces from every line at once.
5. **Save the File:**
    
    - Go to **File → Save** to overwrite your file with the updated content.

---

### **Using Notepad++ Without Regular Expressions:**

If you don’t want to use Regular Expressions:

1. Select all the content (Ctrl + A).
2. Go to the **Edit** menu → Select **Blank Operations** → Click on **Trim Leading Space**.

---

### **Diagram:**


![Pasted image 20241123035007.png](/img/user/Assets/img/Pasted%20image%2020241123035007.png)

---
{"dg-publish":true,"permalink":"/tips-and-tricks/create-the-format-alex-smith-and-bella-jones-in-excel/","noteIcon":"","created":"2024-11-23T04:16:20.562+05:30","updated":"2024-11-23T04:29:45.280+05:30"}
---

### **Method 1: Using a Formula**  #Excel


1. **Enter Your Data:**
    
    - Suppose your list of names is in **Column A** (e.g., `A1:A10`).
2. **Use a Formula to Format the Data:**
    
    - In **Column B**, enter the following formula:
        
        ```
        = "'" & A1 & "',"
        ```
        
    - Press **Enter** to apply it to the first cell in Column B.
3. **Apply the Formula to All Rows:**
    
    - Drag the fill handle (small square at the bottom-right corner of the cell) down to apply the formula to all rows.
4. **Copy and Paste as Values (Optional):**
    
    - If you want to keep only the formatted text (and not the formula), copy the data in Column B.
    - Right-click → Select **Paste Special** → Choose **Values**.

---

### **Method 2: Using CONCATENATE (or TEXTJOIN for multiple cells)**

1. **Enter Your Data:**
    
    - Place the names in **Column A** as before.
2. **Write the Formula:**
    
    - Use the `CONCATENATE` function:
        
        ```
        =CONCATENATE("'", A1, "',")
        ```
        
    - Or for Excel versions supporting `TEXTJOIN` (e.g., Excel 2019/Office 365), combine multiple rows:
        
        ```
        =TEXTJOIN(", ", TRUE, "'" & A1:A10 & "'")
        ```
        
    - For `TEXTJOIN`, press **Ctrl + Shift + Enter** after typing the formula if using an older Excel version.
3. **Drag Down or Apply:**
    
    - Apply the formula as in Method 1.

---

### **Result in Excel:**

Your Column B will look like this:

```
'AlexSmith',
'BellaJones',
'ChrisBrown',
'DianaWhite',
```

Let me know if you need further assistance!
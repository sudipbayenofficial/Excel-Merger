# Excel Merger — Offline Single‑File Web Application

A fully client‑side, single‑file HTML tool that allows you to **merge multiple Excel/CSV files offline**, choose specific columns to keep, preview merged data, and export the result as **XLSX or CSV**.

This tool is designed for **100% offline usage**, with no backend, no server, and no data upload. Everything runs securely inside your browser.

---

## 🚀 Features

### **1. Offline, Single‑File HTML Application**
- Works without internet.
- No server, backend, or installation required.
- All processing happens in the browser using JavaScript.

### **2. Upload Multiple Excel/CSV Files**
- Supports: `.xlsx`, `.xls`, `.csv`
- Drag & Drop upload area
- File cards showing filename and sheet count

### **3. Intelligent Column Handling**
- Automatically collects all unique columns from all files
- Column search bar
- Bulk actions:
  - Select All
  - Unselect All
  - Invert Selection
- **Auto-select Common Columns** (intersection across files)

### **4. Preview Merged Data**
- Preview before downloading
- Pagination controls
- Rows per page selector: 10 / 25 / 50 / 100
- Smooth scrolling and responsive design

### **5. Export as XLSX or CSV**
- Downloads with timestamp pattern:
  ```
  ExcelMerger_YYYYMMDD_HHMMSS.xlsx
  ```
- Completely offline generation

### **6. Clean, Modern UI**
- Professional design
- Branded accent color: `#3031bd`
- Smooth borders, shadows, and typography
- Fully responsive on desktops & laptops

---

## 📁 File Structure

This application is a **single HTML file** that contains:

- HTML layout
- CSS for UI styling
- JavaScript for Excel parsing & merging
- SheetJS library (optionally embedded for full offline support)

---

## 📌 How to Use

### **Step 1: Open the HTML file**
Just double-click the `.html` file to open it in your browser.

### **Step 2: Upload Files**
- Drag & drop multiple Excel/CSV files
- Or click the upload area to browse files

### **Step 3: Select Columns**
- Search columns
- Bulk-select options
- Auto-select common columns

### **Step 4: Click "Generate Preview"**
View merged data with pagination.

### **Step 5: Download Output**
Choose:
- **Download Merged Excel** (.xlsx)
- **Download CSV** (.csv)

---

## 🧩 Making the Tool Fully Offline (Embedding SheetJS)

Right now, the HTML references SheetJS from a CDN:
```html
<script src="https://cdn.jsdelivr.net/npm/xlsx/dist/xlsx.full.min.js"></script>
```

To make the file **100% offline**, do this:

1. Download:
   - https://cdn.jsdelivr.net/npm/xlsx/dist/xlsx.full.min.js

2. Replace the `<script src>` tag with:
   ```html
   <script>
   // Paste entire contents of xlsx.full.min.js here
   </script>
   ```

3. Save the file and reload.

Now the tool is completely standalone.

---

## 🛠 Technology Stack

- HTML5
- CSS3
- Vanilla JavaScript
- **SheetJS** (for Excel parsing & export)

No frameworks. No build system. Pure client-side.

---

## 🧪 Browser Compatibility

Tested and working in:
- Chrome
- Edge
- Firefox
- Brave

(Internet Explorer is **not supported**.)

---

## 📄 License

This project is free to use, modify, and distribute.

---

## 👤 Author
Created for **Sudip Bayen**.

If you want enhancements, such as:
- Column mapping UI
- Deduplication options
- Sorting & filtering
- Embedded SheetJS for full offline mode
- Dark mode or alternative themes
- Upload history / file validation

Feel free to request it!

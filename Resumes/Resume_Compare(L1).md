# Resume_Comparision

## Comparing two resume text sizes :

1. First, install the required library:
```bash
pip install fpdf
```

2. Python's script:

```python
import os
from fpdf import FPDF

def get_file_size(file_path):
    return os.path.getsize(file_path)

def generate_pdf_report(file1_path, file2_path, output_path):
    file1_size = get_file_size(file1_path)
    file2_size = get_file_size(file2_path)
    
    pdf = FPDF()
    pdf.add_page()
    pdf.set_font("Arial", size=12)
    
    pdf.cell(200, 10, txt="Resume Size Comparison Report", ln=True, align='C')
    
    pdf.ln(10)
    pdf.cell(200, 10, txt=f"Size of {os.path.basename(file1_path)}: {file1_size} bytes", ln=True)
    pdf.cell(200, 10, txt=f"Size of {os.path.basename(file2_path)}: {file2_size} bytes", ln=True)
    
    difference = abs(file1_size - file2_size)
    if file1_size > file2_size:
        pdf.cell(200, 10, txt=f"{os.path.basename(file1_path)} is larger by {difference} bytes", ln=True)
    elif file1_size < file2_size:
        pdf.cell(200, 10, txt=f"{os.path.basename(file2_path)} is larger by {difference} bytes", ln=True)
    else:
        pdf.cell(200, 10, txt=f"Both resumes are of the same size.", ln=True)
    
    pdf.output(output_path)

# Provide paths to your resume files and the desired output PDF file
file1 = "path_to_resume1.txt"
file2 = "path_to_resume2.txt"
output_pdf = "comparison_report.pdf"

generate_pdf_report(file1, file2, output_pdf)
```

Replace `path_to_resume1.txt` and `path_to_resume2.txt` with the paths to your actual resume files. The script will then create a `comparison_report.pdf` file in the current directory with the size comparison. Adjust paths accordingly if needed.
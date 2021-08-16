# resume

Repository containing the source code (HTML, CSS, build-scripts) for Anurup
Dey's resume. 

## Dependencies

- `wkhtmltopdf` ( available in most linux package repositories )

## Usage:

1. Create secrets.sh that sets two variables
   `PHNUMBER`,`ADDRESS_CITY`,`CGPA_UNI`,`PERCENTAGE_XII` and `PERCENTAGE_X`.
   Values of these variables will be read while rendering the resume. These
   values are concealed to maintain privacy.

1. Run `./render2pdf` ( Make sure it is executable first, using `chmod +x
   ./render2pdf` if needed. ). It will read `resume.html` and renders it to
   `resume.pdf`. The script is a convenient shorthand with working page size
   and zoom level parameters. 

1. Distribute `resume.pdf`

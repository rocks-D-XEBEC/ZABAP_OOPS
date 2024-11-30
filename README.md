# ZABAP_OOPS
FOR SAP ABAP CODES AND IMPORTANT TIPS 
SAP ABAP 
AP ABAP (Advanced Business Application Programming) is a programming language developed by SAP for building applications within the SAP ecosystem. It is primarily used for developing and customizing SAP modules to meet specific business needs. ABAP is known for its robust integration with SAP's Enterprise Resource Planning (ERP) system.

ABAP IS GENERALLY SIMILAR TO SQL AS ITS SYNTAX IS MORE SIMILAR.

CODING PART IS DONE IN MOSTLY SE38 OF SAP LOGON 

SAMPLE CODE FOR ABAP : 
------------------------------------------------------------------------------------------------------------------------------------------------------------------
REPORT zsample_write_loop.
DATA: lt_numbers TYPE TABLE OF i,
      lv_number  TYPE i.
" Populate internal table with numbers 1 to 10
DO 10 TIMES.
  APPEND sy-index TO lt_numbers.
ENDDO.
" Loop through the table and display each number
LOOP AT lt_numbers INTO lv_number.
  WRITE: / 'Number:', lv_number.
ENDLOOP.
------------------------------------------------------------------------------------------------------------------------------------------------------------------
OUTPUT: 
------------------------------------------------------------------------------------------------------------------------------------------------------------------
Number: 1
Number: 2
Number: 3
UPTO ........
Number: 10
------------------------------------------------------------------------------------------------------------------------------------------------------------------

# List of files 
``` dataview
TABLE without ID
rows.file.link as "Files", dateformat(rows.created, "yy-MMM") AS Saved, Course, rows.summary as Summary
FROM "CourseNotes/2023" 
WHERE !contains(file.name, "Summary")
SORT dateformat(file.day, "yyyy-MM-dd") ASC
GROUP BY course as Course
```

# Hall Ticket Generator

A single-file, offline tool that turns an Excel sheet of students and an exam
timetable into professional, print-ready **PDF hall tickets** — right in your
browser. No install, no server, no account.

Originally built for **Dr M.A Aziz Jr. College Of Science, Phulambri**, but
designed to be reused by any school: just supply your own Excel data and logo.

**Live demo:** https://claude.ai/artifact/NUqA1jC3jJHSpZE2o2qvCE

## How to use it

1. Download `HallTicketGenerator.html` and open it in any browser (Chrome,
   Firefox, Edge) — just double-click the file.
2. Upload your Excel file (see format below). No data yet? Click
   **Download Sample Template** inside the tool to get a starter file.
3. Upload your college logo (optional) — used as the letterhead logo and a
   faint page watermark.
4. Click **Generate Hall Tickets PDF**. The PDF downloads immediately.

Everything runs locally in your browser. Nothing is uploaded to any server —
your student data never leaves your computer.

## What's on each ticket

College logo, name, full address, UDISE code, index number, and academic
year · a faint full-ticket watermark of the college seal · seat number
(assigned automatically) · student name, class ("11th Class" / "12th
Class"), GR No, APAAR ID, parent's name · a blank photo box · the full exam
timetable with the day of the week worked out automatically from the date ·
standard exam instructions · signature lines for Class Teacher and Principal
· an issue-date footer · two tickets per A4 sheet with a cut line between
them.

## Excel format

Three sheets:

**Students** — one row per student

| Name | Class | GR No | Mother's Name | Father's Name | APAAR ID | Seat No |
|---|---|---|---|---|---|---|

`Class` accepts `XI`/`XII` or `11`/`12`. Leave **Seat No** blank — it's
assigned automatically, sequential within each class, ordered by GR No.

**Timetable** — one row per exam day

| Subject | Date | Day | Time |
|---|---|---|---|

`Date` is `dd/mm/yyyy`. Leave **Day** blank and it's worked out from the
date automatically — or fill it in yourself.

**Settings** — two columns, `Key` / `Value`

`College Name`, `Address`, `UDISE Code`, `Index No`, `Academic Year`,
`Exam Title`. (The logo comes from the separate upload, not this sheet.)

## License / Credit

Software by **Khaleeque Hussain**. Free to reuse and adapt for any school.

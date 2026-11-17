# Student Management System (VB.NET)

A Windows desktop application for managing student records, built in Visual Basic (VB.NET) with Visual Studio and a Microsoft SQL Server database. Users can add, view, edit, update, and delete student records through a simple visual interface.

## Features

- **Add** new student records
- **View** all students in a data grid
- **Edit and update** existing student information
- **Delete** records with soft delete, so a record is marked inactive instead of being permanently removed
- **Input validation and exception handling** to catch errors and show clear messages instead of crashing

## Tech Stack

| Area | Tools |
|------|-------|
| Language | Visual Basic (VB.NET) |
| IDE | Visual Studio |
| Database | Microsoft SQL Server Express, SQL Server Management Studio (SSMS) |
| Data Access | ADO.NET (table adapters, datasets, binding sources) |
| Design | Lucidchart (ER diagram) |

## Architecture

The app uses a **three-layer architecture**, which keeps each part of the code focused on one job:

1. **UI layer**: Windows Forms screens the user interacts with
2. **Process (business logic) layer**: handles validation and app rules
3. **Data layer**: SQL Server database, connected through ADO.NET

```
[ UI (Windows Forms) ] → [ Process Layer ] → [ ADO.NET ] → [ SQL Server ]
```

## Database Design

- Designed the database schema with DDL (`CREATE TABLE` statements) in SSMS
- Built an ER diagram in Lucidchart to map out tables and relationships before coding

## Testing

Tested every add, edit, update, and delete action against the SQL Server database. I also tested invalid input, like empty fields and wrong data types, to make sure exception handling showed clear error messages.

## What I Learned

- How to separate an app into UI, logic, and data layers so it's easier to update and debug
- Connecting a desktop UI to SQL Server with ADO.NET table adapters, datasets, and binding sources
- Planning a database with an ER diagram before writing code
- Writing exception handling so the app fails gracefully instead of crashing

## Background

This project started from an earlier console-based Java student management program. I rebuilt it as a visual desktop app in VB.NET with a real SQL Server backend.

## Author

**Riona Bachuwala**

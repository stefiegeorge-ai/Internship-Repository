This MySQL schema manages a library’s books, authors, members, loans, and fines. It supports adding books, tracking loans, and managing late return fines.

Tables

Authors – Author details.

Genres – Unique book categories.

Books – Book info (title, ISBN, author, genre, copies).

Members – Library members.

Loans – Book borrowings with loan/due/return dates.

Fines – Penalties linked to loans, with payment status.

Relationships

Books → Authors, Genres (Many-to-One)

Loans → Books, Members (Many-to-One)

Fines → Loans (One-to-One)

Usage

Run script in MySQL (CREATE DATABASE library;).

Insert authors, genres, books, members.

Track loans and fines using respective tables.

# Music Store Data Analysis - Findings

Project Overview
This project provides a business data analysis of a digital music store using a relational database schema. By executing structured queries in MySQL, the analysis uncovers key insights regarding market performance, consumer music preferences, inventory optimization, and high-value customer segmentation.

Core Technologies Used

Database Management System: MySQL

Interface Tool: MySQL Workbench

SQL Techniques: Multi-table Joins (INNER JOIN, LEFT JOIN), Aggregate Functions (SUM, COUNT, ROUND), Grouping and Ordering (GROUP BY, ORDER BY), Common Table Expressions (CTEs), and Window Functions (ROW_NUMBER).

Database Schema Blueprint

Customer: Stores the buyer's name and Country.

Invoice: The billing receipt that connects a Customer to their order total and purchase date.

InvoiceLine: The individual items on that receipt. It connects the Invoice to the specific Track sold.

Track: The individual song, its price, and its format. It connects to the Album and Genre.

Genre: The musical style label (like Rock or Pop).

Album: The collection of songs, which connects back to the Artist.

Artist: The creator or band who made the music.

Query Findings

Query 1: Market Analysis (Revenue by Country)

USA: $523.74 (Highest revenue market)

Canada: $303.96 (Second highest)

France: $195.10 (Third highest)

Brazil: $190.10 (Fourth highest)

Query 2: Product Management (Top-Selling Genres)

Rock: 835 tracks sold (Dominates the store completely)

Latin: 386 tracks sold

Metal: 264 tracks sold

Alternative & Punk: 244 tracks sold

Query 3: Customer Segmentation (Top Spenders per Country)

Czech Republic VIP: Helena Holy ($49.62 spent)

USA VIP: Richard Cunningham ($47.62 spent)

Canada VIP: Luis Rojas ($46.62 spent)

Brazil VIP: Ladislav Kovacs ($45.62 spent)

Query 4: Inventory Optimization (Unsold Tracks)

Total Unsold Catalog: 1,519 tracks in the database have never been bought by any customer.

Sample Unsold Tracks: "Amanda", "Talk About Love", "Shine On You Crazy Diamond".

Query 5: Temporal Trends (Monthly Sales)

Highest Revenue Month: January ($119.88 total sales)

Second Highest Month: April ($100.98 total sales)

Lowest Revenue Month: October ($74.24 total sales)

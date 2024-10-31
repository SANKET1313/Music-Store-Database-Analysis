
# Music Store Database Analysis

Project Overview

This project analyzes sales data from a music store to uncover insights about customer preferences, sales trends, and inventory management. The goal is to provide recommendations based on the analysis that can help optimize sales strategies.


Dataset Description

The image depicts a database schema commonly used in a music-related application, likely for managing artists, albums, tracks, playlists, and invoices. Here's an overview of the main entities and their relationships:

Entities:

Artist: Represents musicians or bands. Contains fields like ArtistId and Name.

Album: Represents albums containing tracks. Related to Artist by ArtistId. Fields include AlbumId, Title, and ArtistId.

Track: Represents individual music tracks. Linked to Album and includes fields such as TrackId, Name, MediaTypeId, GenreId, Composer, Milliseconds, Bytes, and UnitPrice.

Playlist: Collections of tracks. Contains PlaylistId and Name.

PlaylistTrack: A junction table connecting Playlist and Track, with PlaylistId and TrackId.

MediaType: Details about media formats (e.g., audio files). Includes MediaTypeId and Name.

Genre: Represents categories of music. Consists of GenreId and Name.

Sales and Billing Entities:

Customer: Represents users or clients. Contains fields like CustomerId, FirstName, LastName, Address, City, Email, etc.

Invoice: Represents purchase records. Fields include InvoiceId, CustomerId, InvoiceDate, and billing details.

InvoiceLine: A line item in an invoice, connecting Invoice and Track. Contains InvoiceLineId, InvoiceId, TrackId, UnitPrice, and Quantity.

Relationships:

One-to-Many: For example, one artist can produce multiple albums, and one album can have multiple tracks.

Many-to-Many: For instance, a playlist can contain many tracks and a track can appear in many playlists, managed through the PlaylistTrack table.

Linking Sales to Customers: Each invoice is associated with a single customer, and each invoice can have multiple line items corresponding to different tracks purchased.

This schema provides a comprehensive structure to manage a music catalog, including artist information, track listings, playlists for organization, and invoice records for sales transactions.

Technologies Used

Database: SQL
Tools: Postgresql

Analysis

This database structure helps the music store efficiently manage its operations.

It allows for easy access to music data for customers, simplifies the sales process, and provides a clear organization of music-related information.

Overall, it supports a smooth experience for both the store and its customers.

Results

The design allows for easy addition of new artists, albums, and tracks without disrupting existing data, making it ready for future growth.

Managers can generate reports on customer purchases, popular tracks, and overall sales, helping them make informed business decisions.

The database keeps all music-related information neatly organized, making it easy to find details about artists, albums, tracks, and customers.
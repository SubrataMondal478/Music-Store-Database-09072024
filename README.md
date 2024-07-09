# Music-Store-Database-09072024

Project Overview
The Music Store Database Project is designed to manage and analyze data for a music retail business. The database keeps track of artists, albums, genres, tracks, customers, orders, playlists, suppliers, and inventory. This relational database facilitates efficient data management, querying, and reporting for various business operations, such as tracking sales, managing inventory, and analyzing customer preferences.

Key Entities and Relationships
Artists

Attributes: ArtistID, Name, Country
Description: Stores information about musical artists.
Relationships: An artist can have multiple albums.
Albums

Attributes: AlbumID, Title, ArtistID, ReleaseDate
Description: Stores information about music albums.
Relationships: An album is created by an artist and contains multiple tracks.
Genres

Attributes: GenreID, GenreName
Description: Stores different music genres.
Relationships: Each track belongs to a genre.
Tracks

Attributes: TrackID, Title, AlbumID, GenreID, Length
Description: Stores information about individual music tracks.
Relationships: Each track belongs to an album and a genre, and can appear in multiple orders and playlists.
Customers

Attributes: CustomerID, FirstName, LastName, Email, PhoneNumber
Description: Stores customer information.
Relationships: Customers place orders and create playlists.
Orders

Attributes: OrderID, CustomerID, OrderDate
Description: Stores information about customer orders.
Relationships: Each order is placed by a customer and includes multiple order details (tracks).
OrderDetails

Attributes: OrderDetailID, OrderID, TrackID, Quantity, Price
Description: Stores details of each order, including tracks purchased.
Relationships: Each order detail is linked to an order and a track.
Playlists

Attributes: PlaylistID, Name, CustomerID
Description: Stores information about customer playlists.
Relationships: Each playlist is created by a customer and contains multiple tracks.
PlaylistTracks

Attributes: PlaylistTrackID, PlaylistID, TrackID
Description: Stores tracks included in playlists.
Relationships: Each playlist track is linked to a playlist and a track.
Suppliers

Attributes: SupplierID, Name, ContactName, ContactEmail
Description: Stores supplier information.
Relationships: Suppliers provide albums.
Inventory

Attributes: InventoryID, AlbumID, SupplierID, Quantity
Description: Stores inventory details for albums.
Relationships: Inventory items are linked to albums and suppliers.
Use Cases
Sales Tracking

Track customer orders and sales details.
Analyze sales by artist, album, genre, and track.
Inventory Management

Monitor inventory levels and manage supplier relationships.
Analyze inventory to ensure stock availability and reduce overstock.
Customer Management

Store and manage customer information.
Track customer preferences and order history for targeted marketing.
Playlist Management

Allow customers to create and manage playlists.
Analyze popular tracks and playlists for marketing insights.
Benefits
Efficiency: Streamlines data management and retrieval processes.
Insights: Provides valuable insights into sales trends, inventory levels, and customer preferences.
Scalability: Supports the growth of the music store by accommodating more data and complex queries.
Integration: Facilitates integration with other systems for reporting and business intelligence.
This project showcases the implementation of a comprehensive database system for a music store, highlighting the importance of organized data management in enhancing business operations and decision-making.

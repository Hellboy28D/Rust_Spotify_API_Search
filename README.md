🎵 Rust Spotify API Search

Overview

Rust Spotify API Search is a command-line application built using Rust that integrates with the Spotify Web API to search and retrieve music information in real time.

The application allows users to search for tracks using a query string and displays detailed information including track name, album details, artist names, popularity information, and direct Spotify links.

This project was created to explore API integration, asynchronous programming, JSON deserialization, and command-line application development using Rust.

⸻

Project Objectives

The main goals of this project are:

* Learn Rust through hands-on implementation
* Understand API communication
* Work with asynchronous programming using Tokio
* Parse JSON responses using Serde
* Build a command-line application
* Practice handling HTTP requests and authentication

⸻

Features

✅ Search Spotify tracks using custom keywords

✅ Connect to Spotify Web API

✅ Authentication using Bearer Token

✅ Asynchronous HTTP requests using Reqwest

✅ JSON response parsing with Serde

✅ Display track information

✅ Display album information

✅ Display artist information

✅ Generate direct Spotify links

✅ Error handling for invalid tokens and failed requests

⸻

Technologies Used

Language

* Rust

Libraries and Crates

* Reqwest
* Tokio
* Serde
* Serde JSON

⸻

Project Structure

Rust_Spotify_API_Search/

├── Cargo.toml

├── Cargo.lock

├── src/

│ └── main.rs

├── README.md

└── .gitignore

⸻

How It Works

The application follows this workflow:

Step 1: User provides input

The user passes:

* Search query
* Spotify access token

Example:

cargo run "Imagine Dragons" YOUR_ACCESS_TOKEN

⸻

Step 2: Build API Request

The application creates a request URL:

https://api.spotify.com/v1/search?q=query&type=track,artist

⸻

Step 3: Authenticate Request

The request includes:

Authorization: Bearer ACCESS_TOKEN

⸻

Step 4: Fetch Data

Reqwest sends an asynchronous request to Spotify servers.

⸻

Step 5: Deserialize JSON

Serde converts Spotify JSON responses into Rust structs:

* Track
* Album
* Artist
* ExternalUrls

⸻

Step 6: Display Results

Example output:

Believer
Evolve
Imagine Dragons
https://open.spotify.com/track/...
---------

⸻

Concepts Practiced

This project helped strengthen understanding of:

Rust fundamentals

* Structs
* Vectors
* Iterators
* Ownership
* Borrowing
* Error handling

API development concepts

* REST APIs
* HTTP methods
* Headers
* Authentication
* JSON parsing

Async Programming

Using:

#[tokio::main]
async fn main()

for asynchronous execution.

⸻

Installation

Clone the repository:

git clone https://github.com/Hellboy28D/Rust_Spotify_API_Search.git

Move into project directory:

cd Rust_Spotify_API_Search

Install dependencies:

cargo build

Run the application:

cargo run "Adele" YOUR_ACCESS_TOKEN

⸻

Example Output

Rolling in the Deep
21
Adele
https://open.spotify.com/track/xxxxx
---------

⸻

Future Improvements

🚀 Search albums and playlists

🚀 Interactive CLI interface

🚀 Colored terminal output

🚀 Token automation and refresh support

🚀 Pagination support

🚀 Better error handling

🚀 Search filters

🚀 Package as a reusable CLI tool

⸻

Learning Outcomes

This project provided practical experience with:

* Rust development
* API consumption
* Async programming
* Struct design
* JSON deserialization
* CLI application design
* Authentication handling

⸻

Author

Divakr Dayas

If you found this project interesting, feel free to star the repository and share your feedback.

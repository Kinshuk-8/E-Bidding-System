
#                           E-Bidding

An innovative online auction platform that brings together buyers and sellers for real-time bidding on products. Built with a modern JavaScript stack, this project harnesses the power of Express.js, MongoDB, Node.js, and React to offer a seamless bidding experience.

------------------------------------------------------------

## Introduction

Welcome to E-Bidding! This repository houses an online bidding platform where users can create auctions, place bids, and participate in a dynamic marketplace. The project is divided into a backend powered by Express.js and MongoDB and a frontend built with React. The system also integrates real-time bid updates using Socket.io and scheduled auction checks using Node Cron. Whether you are a seller wanting to auction items or a buyer looking for great deals, E-Bidding delivers a robust and user-friendly solution.

------------------------------------------------------------

## Features

- **Auction Management**  
  - Create auctions with titles, descriptions, images, and bid ranges.
  - Manage auction status with start and end times.
  - Real-time auction updates using WebSockets.

- **Bidding System**  
  - Place bids on active and upcoming auctions.
  - Validate bid amounts to ensure they exceed the current highest bid.
  - Maintain detailed bidding history for each auction.

- **User Authentication & Profile**  
  - Secure login and profile management.
  - Distinct experiences for regular users and admins.
  
- **Payment Processing**  
  - Record payments and view payment history for completed auctions.
  
- **Image Uploads**  
  - Utilize Cloudinary for image uploads when creating auctions.

- **Admin Dashboard**  
  - Manage users, auctions, and approve/reject auction listings.
  
- **Scheduled Auction Checker**  
  - Automatically check for ended auctions every minute and declare winners.

------------------------------------------------------------

## Usage

E-Bidding is designed to be easy to use for both sellers and buyers:

1. **For Sellers:**  
   - Sign up or log in.
   - Navigate to the “Create Auction” page.
   - Fill in the auction details including title, description, starting bid, start and end times, and upload an image.
   - Submit the form to list your auction.

2. **For Buyers:**  
   - Log in and browse ongoing or upcoming auctions from the home page.
   - Click on an auction to view detailed information.
   - Place a bid through the bid input; the system will validate and update the bid in real time.

3. **Admin Usage:**  
   - Admin users have additional options to manage users and auctions.
   - Access the admin dashboard to approve, reject, or delete auctions.



## Configuration

Before running the system, make sure to set up the environment variables as shown in the table below:

| Variable Name                  | Description                                  | Example Value                           |
| ------------------------------ | -------------------------------------------- | --------------------------------------- |
| PORT                           | Server port for the backend                  | 4000                                    |
| MONGO_URI                      | MongoDB connection string                    | mongodb://localhost:27017/ebidding      |
| CLOUDINARY_CLOUD_NAME          | Cloudinary cloud name for image uploads      | your-cloud-name                         |
| CLOUDINARY_API_KEY             | API key for Cloudinary                       | your-api-key                            |
| CLOUDINARY_SECRET_KEY          | Secret key for Cloudinary                    | your-secret-key                         |
| JWT_SECRET                     | Secret for JSON Web Token signing            | your-jwt-secret                         |

> Make sure to create a .env file at the backend root with the above variables configured.

------------------------------------------------------------

## Requirements

To successfully run E-Bidding, please ensure you have the following installed:

- **Node.js** (Version 14 or higher recommended)  
- **npm** or **yarn** package manager  
- **MongoDB** server (local or remote instance)  
- A Cloudinary account for handling image uploads  
- Internet connection for API requests (e.g., Cloudinary and any other third-party integrations)

------------------------------------------------------------

## Installation

Follow these steps to install and run the project locally:

1. **Clone the repository:**

   ------------------------------------------------------------
   git clone https://github.com/Kinshuk-8/E-Bidding-System
   ------------------------------------------------------------

2. **Backend Installation:**

   - Navigate to the backend directory:
     
     ------------------------------------------------------------
     cd E-Bidding/Backend
     ------------------------------------------------------------
     
   - Install the backend dependencies:
     
     ------------------------------------------------------------
     npm install
     ------------------------------------------------------------

   - Create a .env file in the Backend folder and add the required environment variables yourself as detailed above.
  
   - Start the backend server:
     
     ------------------------------------------------------------
     npm run start
     ------------------------------------------------------------

3. **Frontend Installation:**

   - Navigate to the frontend directory:
     
     ------------------------------------------------------------
     cd E-Bidding/frontend
     ------------------------------------------------------------
     
   - Install the frontend dependencies:
     
     ------------------------------------------------------------
     npm install
     ------------------------------------------------------------
     
   - Start the frontend development server:
     
     ------------------------------------------------------------
     npm start
     ------------------------------------------------------------

4. **Access the Application:**

   - The backend API will run on the port specified in your .env (default is 4000).
   - The frontend will typically run on port 3000. Open your browser and navigate to http://localhost:3000 to start using E-Bidding 🚀

------------------------------------------------------------

Enjoy exploring the platform, and happy bidding! 🙌

------------------------------------------------------------

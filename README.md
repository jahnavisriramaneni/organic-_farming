Organic Farming App
A Flutter application designed to provide information and guidance on organic farming practices, including low-budget home farming, key techniques, and plant-specific details. Users can log in to access a personalized dashboard with advanced features.

Table of Contents
Features

Getting Started

Prerequisites

Installation

Running the App

Project Structure

Screenshots (Placeholder)

Future Enhancements

Features
Homepage:

Introduction to organic farming.

Advantages of organic farming.

Image gallery showcasing organic farming.

Navigation to "Low-Budget Organic Farming" page.

Authentication (Login/Sign Up):

Dedicated Login and Sign Up pages.

Seamless navigation between authentication pages.

(Currently simulated login/signup, no backend integration).

Low-Budget Organic Farming Page:

Detailed information on how to do organic farming at home or on a low budget.

Principles for budget organic farming.

General compost and organic fertilizer needs.

DIY organic fertilizer recipes.

User Dashboard (Post-Login):

Welcome message and overview.

Plant Search: Search for specific plants to get details on their fertilizer needs and how organic farming benefits their growth.

Key Organic Farming Techniques: Interactive cards displaying core organic farming practices (e.g., Composting, Crop Rotation, Natural Pest Control). Tapping a card shows a brief description (currently via SnackBar).

Organic Fertilizer Preparation: Detailed instructions for preparing various homemade organic fertilizers.

Getting Started
Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

Prerequisites
Flutter SDK (version 3.8.1 or higher recommended as per pubspec.yaml)

Android Studio (for Android emulator/device setup) or VS Code with Flutter extension.

Git (for cloning the repository)

Installation
Clone the repository:

git clone [your-repository-url]
cd organic_farming_app

(Replace [your-repository-url] with the actual URL if this project is hosted on Git).

Install dependencies:
Navigate to the project root directory and run:

flutter pub get

Add Custom Fonts:
This project uses the 'Montserrat' font.

Download the Montserrat font files (e.g., Montserrat-Regular.ttf, Montserrat-Bold.ttf) from Google Fonts.

Create a fonts directory in the project root (organic_farming_app/fonts).

Place the downloaded .ttf files into this fonts directory.

Ensure your pubspec.yaml has the font declaration under the flutter: section:

flutter:
  uses-material-design: true
  fonts:
    - family: Montserrat
      fonts:
        - asset: fonts/Montserrat-Regular.ttf
        - asset: fonts/Montserrat-Bold.ttf
          weight: 700

(Verify uses-material-design: true appears only once).

Add Local Images (if applicable):
If you plan to re-add images to the homepage or other sections, create an assets/images directory in the project root and place your image files there. Remember to declare the asset folder in pubspec.yaml:

flutter:
  # ...
  assets:
    - assets/images/

Running the App
Connect a device or start an emulator:
Ensure you have an Android emulator running, an iOS simulator, or a physical device connected and recognized by Flutter (flutter devices).

Run the application:

flutter run

This will launch the app on your selected device/emulator.

Project Structure
The core Dart files are located in the lib/ directory:

organic_farming_app/
├── lib/
│   ├── main.dart             # Main entry point, app theme, and route definitions.
│   ├── home_page.dart        # The public-facing homepage with advantages and image gallery.
│   ├── login_page.dart       # User login interface.
│   ├── signup_page.dart      # User registration interface.
│   ├── low_budget_farming_page.dart # Page detailing low-budget organic farming methods.
│   ├── dashboard_page.dart   # User's personalized dashboard with plant search, techniques, and fertilizer prep.
│   └── technique_detail_page.dart # Displays detailed info for a specific organic technique (accessed from Dashboard).
├── pubspec.yaml              # Project dependencies and asset declarations.
├── README.md                 # This file.
└── ... (other Flutter project files)

Screenshots (Placeholder)
Add screenshots of your app's main pages here.

Future Enhancements
Backend Integration: Implement actual user authentication (e.g., Firebase Authentication).

Dynamic Content: Fetch plant data, technique details, and fertilizer recipes from a backend database.

User Profiles: Allow users to manage their profiles and preferences.

Interactive Guides: Add step-by-step guides for farming techniques.

Community Features: Forums, sharing tips, or connecting with other organic farmers.

Notifications: Reminders for watering, fertilizing, or harvesting.

More Plant Data: Expand the _organicPlantData with a wider variety of plants.

Visual Enhancements: Further refine UI/UX, add animations, and improve responsiveness across devices.

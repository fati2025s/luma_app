# Luma app

**luma app** modern user interface for managing your smart home devices.

**luma app** is a mobile application developed with Flutter/Dart. This repository contains only the Frontend code, focusing on the UI/UX, state management, and client-side logic required to communicate with a separate Smart Home Backend API.

# Project Overview (Frontend Focus)

This project demonstrates proficiency in building a complex, data-intensive, and highly reactive user interface using Flutter. The frontend is responsible for displaying real-time home status, sending control commands, and managing user-defined automation scenarios.

# Key Flutter Frontend Features

Real-time Dashboard: Displays immediate status updates for all connected sensors (temperature, humidity, light, security status) with fast, responsive UI updates.

Intuitive Device Control: Sends control commands (on/off, temperature setting, color changes) to the devices via the API.

Automation Management: Allows users to easily create, edit, and toggle complex home automation routines (Scenarios/Scenes).

Modern & Adaptive UI: Built with Flutter's widget system for a beautiful, responsive, and cross-platform experience (Mobile/Tablet).

Modular Architecture: Utilizes a clean code structure for easy maintenance and future feature scalability.

## Features & Screenshots

### Welcome Page
![Welcome Page](https://github.com/fati2025s/luma_app/tree/main/images/screenshots/1.jpg)

### Login & Signup (OTP/Phone Number Based): 

![login & signup1](https://github.com/fati2025s/luma_app/tree/main/images/screenshots/2.jpg)
The authentication process is handled via phone number verification (OTP). The Frontend implements the following crucial steps:

**OTP Request** : Manages sending the phone number to the Backend API for code generation.
![login & signup2](https://github.com/fati2025s/luma_app/tree/main/images/screenshots/4.jpg)

**Loading State Management**: 
![loading](https://github.com/fati2025s/luma_app/tree/main/images/screenshots/3.jpg)

Crucially, a loading/spinner indicator is displayed during all server-side operations (e.g., OTP dispatch and final token validation). This ensures the user knows the application is actively waiting for server response, improving perceived performance and preventing confusion.

**Verification**: Handles receiving and validating the OTP against the server for successful session establishment.

**Session Management**: Upon successful verification, the app securely stores the authentication token retrieved from the backend to maintain the user session.

**Home Screen**
![Home Page](https://github.com/fati2025s/luma_app/tree/main/images/screenshots/5.jpg)

The home page is the user's gateway to managing locations and modules in the application. It provides the user with a collection of essential information and quick access features.
Initial loading: When entering the page, the page is displayed in Loading mode until the information is fully received from the server to prevent incomplete or messy display of information.

Scrolling capability: After successful loading, the page has vertical scrolling capability and the user can navigate between locations.

Location Management Section
Information about user-defined locations is displayed in separate boxes:

View Locations: Each box (card) contains information about a saved location (such as the location name).

Access Modules: By clicking on each location box, the user is redirected to the internal page of that location to view and manage the list of modules installed there.

**Adding New Location**
![Add Location](https://github.com/fati2025s/luma_app/tree/main/images/screenshots/6.jpg)

Empty Add Box: There is a specific empty box or button on the page.

Define New Location: By clicking on this box, a special menu opens that allows the user to define new locations for installing and categorizing modules in the application.

**Menu**
![Menu](https://github.com/fati2025s/luma_app/tree/main/images/screenshots/9.jpg)

Clicking on the three-line icon (Hamburger Menu) at the top of the page will open a quick access drop-down menu.

**Location Page**
![Location Page](https://github.com/fati2025s/luma_app/tree/main/images/screenshots/8.jpg)

The Location page is the heart of managing your smart devices in a specific location (such as "Kitchen" or "Living Room"). From this page, you can view and manage the status of your modules.

Modules List: All modules you have previously assigned to this location (such as lighting modules, air conditioners, or other smart products) are displayed in a list or as individual cards.

Empty State:

If you have not added any modules to this location yet, the page will display a friendly Empty State message.

This message encourages the user to install their first module using the Add button.

**َAdd Modules**
![Add modules](https://github.com/fati2025s/luma_app/tree/main/images/screenshots/7.jpg)

Add a new module (Add Module)
Add button (➕): At the top of the page, there is a button (usually with a plus symbol or ➕).

Open the Add menu: Clicking on this button opens an access menu or modal.
Menu Features: This menu allows you to:

Select the type of module you want (e.g., lighting module or cooling module).

Add and activate the new module to the current location by scanning the QR/barcode or manually entering the activation code (Active Code).

**information**
![User Page](https://raw.githubusercontent.com/fati2025s/luma_app/main/images/screenshots/10.jpg)

# 💳 TrackMySpend - Track Your Subscription Expenses 💳
## 🌟 Table of Contents
- [Overview](#-overview-)
- [Workflow](#-workflow-)
- [Technologies Used](#-technologies-used-)
- [Important Implementation Areas](#-important-implementation-areas-)
- [Key Features](#-key-features-)
- [Flutter-Specific Considerations](#-flutter-specific-considerations-)
- [Screenshots](#-screenshots-)
- [Ending Note](#-ending-note-)

<!--Line-->
<img src="https://user-images.githubusercontent.com/your_image_url/expense-tracker.gif" width="900">

## 🌟 Overview 🌟
*TrackMySpend* is a cross-platform mobile application built using *Flutter*. It helps users manage their subscription-based app expenses and track upcoming bills. The app includes functionalities such as:

- *Subscription Tracking*: Monitor your spending for each subscription plan.
- *Category-Wise Spending*: See how much you’re spending in different categories.
- *Add New Subscription*: Easily input new subscription details.
- *Calendar Schedule*: Keep track of upcoming bills and payments.
- *Card Saver*: Safely store your payment card information.
- *Profile Management*: Manage your account, subscriptions, and settings.

The app features a modern UI and smooth user experience, with a *bottom navigation bar* for easy access to key sections of the app.

## 🛠️ Workflow 🛠️
Here’s how the app will work and what you need to focus on:

### 1. *Welcome Screen*
   - Upon opening the app, the user is greeted with a *welcome screen* that provides two options: "Get Started" (for new users) and "I Have an Account" (for returning users).
   - This will include basic UI components such as *buttons, texts, and icons*.

### 2. *User Authentication*
   - If the user chooses "Get Started," they will be taken to a *sign-up screen*. Upon successful sign-up, they will be redirected to the home screen.
   - For returning users, the "I Have an Account" option leads to the *sign-in screen* where users can log in using their credentials (email/password or social login).

### 3. *Home Screen*
   - After authentication, the user is directed to the *Home Screen* with a *bottom navigation bar*.
   - The home screen will show a *spending bar* for the current month, displaying total spending and upcoming bills for subscriptions.
   - This will require integration with a *charting library* (e.g., *fl_chart* or *syncfusion_flutter_charts*) to visualize the data.

### 4. *Category-Wise Spending*
   - The second section of the bottom navigator displays a breakdown of spending by *subscription categories* (e.g., streaming, utilities, entertainment, etc.).
   - A *ListView* or *GridView* can be used to display the categories with details like *spending amounts* and *category names*.

### 5. *Add New Subscription*
   - In this section, users can *add new subscriptions* by inputting details such as the app name, amount, billing cycle, etc.
   
### 6. *Calendar Schedule*
   - This section will display the *calendar* view of upcoming bills and payments. The calendar will highlight the dates when a bill is due.
   - You can use *Flutter’s calendar packages* like *table_calendar* or *flutter_calendar_carousel* to implement this.

### 7. *Card Saver*
   - Users can save their *credit/debit card details* securely in this section.
   - It’s crucial to implement *security measures* like *encryption* to store card details safely, and you may use libraries such as *flutter_secure_storage* for this.

### 8. *Profile Management*
   - Users can manage their profile information, including their name, email, and password, or add additional subscription plans.
   - Use standard *profile management* components like *avatar, input fields, and buttons*.

## ⚙️ Technologies Used ⚙️
1. *Flutter*
   - Flutter will be used to develop the app’s *UI* for both Android and iOS, ensuring a consistent experience across platforms.
   
2. *Dart*
   - Dart is the primary programming language used in Flutter. It’s essential to have a good understanding of Dart for building the app’s logic.

3. *Flutter Secure Storage*
   - This package will be used to *encrypt and store sensitive data* like payment card information securely.

4. *Charting Library (e.g., fl_chart)*
   - Use a charting library to display spending data and trends on the home screen.

5. *Table Calendar / Flutter Calendar Carousel*
   - Use a calendar package for the *upcoming bills calendar view*.

## 📸 Screenshots 📸

Here are some example mockup screenshots for various screens of the app to visualize how it might look:-
<table>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/a46cea77-f76c-4bbc-b87e-fa99977968aa" width="150"/></td>
    <td><img src="https://github.com/user-attachments/assets/a35e1a6c-35c7-403a-949f-639c2cc34923" width="150"/></td>
    <td><img src="https://github.com/user-attachments/assets/3f85225f-dde3-4fae-82e6-037b97cb9101" width="150"/></td>
  </tr>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/55eb25d8-236f-4dd2-a7bb-08068d69248b" width="150"/></td>
    <td><img src="https://github.com/user-attachments/assets/6c616a1b-70e1-42cf-8bd4-337dc92fb3a4" width="150"/></td>
    <td><img src="https://github.com/user-attachments/assets/d35b90ad-d91c-4910-82e2-f52e5929aed9" width="150"/></td>
  </tr>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/883c1b63-3acc-46c3-bb81-0c5d4a3076ff" width="150"/></td>
    <td><img src="https://github.com/user-attachments/assets/963069c9-8f15-4fd1-9dae-278117fdb42a" width="150"/></td>
    <td><img src="https://github.com/user-attachments/assets/a9c09ae9-b589-47d5-907d-9718f07120fb" width="150"/></td>
  </tr>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/cadd2836-15a7-4b3f-840a-6e4253bec874" width="150"/></td>
    <td><img src="https://github.com/user-attachments/assets/52fcaf02-913d-4a6f-bcc7-5209d17525ef" width="150"/></td>
  </tr>
</table>

## 📄 Ending Note
*TrackMySpend* is designed to make tracking subscription-based expenses simple and efficient. By leveraging Flutter, we ensure that this app will be cross-platform, providing a seamless experience on both Android and iOS. Keep security, user experience, and performance optimization in mind as you develop this app, and you’ll have a powerful tool for managing subscription spending!


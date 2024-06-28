# Dark_mode
# Light and Dark Mode Android Application

## Overview

This Android application showcases the implementation of light and dark mode themes. It demonstrates how to switch between these modes dynamically and how to ensure a consistent user experience across both themes.

## Features

- **Dynamic Theme Switching**: Users can toggle between light and dark modes.
- **Consistent UI**: Ensures that all UI elements are properly themed in both modes.
- **Persistent Theme State**: Remembers the user's theme preference even after the app is closed and reopened.



## Screenshots

<p align="center">
  <img src="https://github.com/imDhiraj/Dark_mode/assets/93609511/a2fce683-d721-4a5e-a56d-cfef07495813" alt="Light Mode" width="45%" style="margin-right: 20px;"  />
   
  <img src="https://github.com/imDhiraj/Dark_mode/assets/93609511/4f6443b7-a386-467f-8ffe-bf062e5f5728" alt="Dark Mode" width="45%" />
</p>

## Installation

1. Clone the repository:
   https://github.com/imDhiraj/Dark_mode.git

2. Open the project in Android Studio.

3. Build and run the application on an Android device or emulator.

## Code Structure

- `MainActivity.java` - The main activity handling the theme switch.
- `styles.xml` - Contains the definitions for both light and dark themes.
- `themes.xml` - Defines the theme resources.
- `colors.xml` - Specifies the color values for light and dark themes.

## How It Works

The application uses Android's built-in theme support to switch between light and dark modes. By defining separate resources for each theme, the app can dynamically change its appearance based on the user's preference.

### Key Code Snippets

#### Switching Themes
```java
public void switchTheme(boolean isDarkMode) {
    if (isDarkMode) {
        AppCompatDelegate.setDefaultNightMode(AppCompatDelegate.MODE_NIGHT_YES);
    } else {
        AppCompatDelegate.setDefaultNightMode(AppCompatDelegate.MODE_NIGHT_NO);
    }
    recreate();
}

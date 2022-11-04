[![Current Release](https://img.shields.io/github/release/scaarup/aula/all.svg?style=plastic)](https://github.com/scaarup/aula/releases) [![Github All Releases](https://img.shields.io/github/downloads/scaarup/aula/total.svg?style=plastic)](https://github.com/scaarup/aula/releases) [![hacs_badge](https://img.shields.io/badge/HACS-Custom-41BDF5.svg?style=plastic)](https://github.com/scaarup/aula)

# Aula

This is a custom component for Home Assistant to integrate Aula. It is very much based on the great work by @JBoye at https://github.com/JBoye/HA-Aula. However this "rewrite" comes with new features like:

- Installable/updatable via HACS
- "Ugeplaner"
  
  As they can be quite large in size, we save these as html, which can be included in your dashboard via the webpage card.
- School schedules as Home Assistant calendars. 
One calendar entity per child. Teacher initials are displayed and substitute teacher is highlighted with full name.

   ![image](https://user-images.githubusercontent.com/8055470/199254249-3bf441bc-7dce-4f5d-a809-d119d20a7b2b.png)
- Lots of small fixes and optimizations

## Installation

### HACS

- Add https://github.com/scaarup/aula as a custom repository
- Search for and install the "Aula" integration.
- Restart Home Assistant.

#### Manual installation

- Download the latest release.
- Unpack the release and copy the custom_components/aula directory into the custom_components directory of your Home Assistant installation.
- Restart Home Assistant.

## Setup

- Add the following to your configuration.yaml:

```
aula:
  username: <your unilogin username>
  password: <your unilogin password>
  schoolschedule: true # If you want "skoleskema" as calendars
```

- Restart Home Assistant.

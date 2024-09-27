# Simple JS Carousel

This project is a **Simple JavaScript Carousel** designed to showcase a rotating series of items (like images or text slides) using basic JavaScript, HTML, and CSS. It provides smooth transitions between slides and is highly customizable with the use of data attributes.

## Features

- **Automatic sliding** of items with customizable delays.
- **Manual navigation** through previous and next buttons.
- **Indicator buttons** to directly jump to specific slides.
- **Customizable slide speed** and ability to enable or disable auto-sliding.
- **Reduced motion** support for users who prefer less animation.

## How the Carousel Works

A carousel typically displays a series of "slides" (usually images or text) that can be navigated through buttons, indicators, or automatically after a set delay. This simple JS Carousel includes:
- Previous and Next buttons for manual navigation.
- Indicators (small buttons) that let users jump directly to any slide.
- Automatic cycling through the slides with customizable speed and delay.

The carousel component is initialized on any element with the `.carousel` class and is powered entirely by JavaScript.

## Carousel Structure

To create a working carousel with this project, your HTML structure should look something like this:

```html
<div id="myCarousel" class="carousel" data-auto="true" data-delay="3000" data-speed="600" data-disable-indicators="false">
    <div class="carousel-item active">
        <img src="image1.jpg" alt="Slide 1">
    </div>
    <div class="carousel-item">
        <img src="image2.jpg" alt="Slide 2">
    </div>
    <div class="carousel-item">
        <img src="image3.jpg" alt="Slide 3">
    </div>
    
    <!-- Navigation Buttons -->
    <button class="prev-btn">Previous</button>
    <button class="next-btn">Next</button>
</div>
```

### Explanation:

- **`.carousel`**: The container that wraps all slides. This is where the JavaScript functionality is applied.
- **`.carousel-item`**: Each slide is wrapped in this class. The first slide should have the `active` class initially.
- **Previous and Next buttons**: These buttons allow the user to navigate manually between slides.

### Indicator Buttons (Optional)

If indicators are enabled (more on this below), the carousel will automatically generate small clickable buttons that allow users to jump to a specific slide.

## Customization Using Data Attributes

The carousel can be customized through several `data-*` attributes that modify its behavior:

### 1. `data-auto="true"`

- **Purpose**: Enables or disables automatic sliding between items.
- **Options**:
  - `true`: Enables auto-slide functionality.
  - `false`: Disables auto-slide.
  
  In the example:
  ```html
  data-auto="true"
  ```
  The carousel will automatically move to the next slide after a certain delay.

### 2. `data-delay="3000"`

- **Purpose**: Sets the delay (in milliseconds) between automatic slide transitions.
- **Value**: The delay is specified in milliseconds (e.g., `3000` for a 3-second delay).
  
  In the example:
  ```html
  data-delay="3000"
  ```
  The carousel will wait for 3 seconds before sliding to the next item.

### 3. `data-speed="600"`

- **Purpose**: Defines the transition speed (in milliseconds) of the sliding animation between items.
- **Value**: The transition speed is specified in milliseconds (e.g., `600` for a 0.6-second transition).

  In the example:
  ```html
  data-speed="600"
  ```
  The sliding animation will take 0.6 seconds to complete.

### 4. `data-disable-indicators="false"`

- **Purpose**: Enables or disables the indicator buttons that let users jump directly to a specific slide.
- **Options**:
  - `true`: Disables the indicators.
  - `false`: Enables the indicators.

  In the example:
  ```html
  data-disable-indicators="false"
  ```
  The carousel will display indicator buttons that allow users to select a specific slide.

## Usage

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/Jackstar-Git/Simple-JS-Carousel
   cd Simple-JS-Carousel
   ```

2. **Modify the HTML**:
   Structure your HTML as shown in the examples above, and customize the data attributes according to your needs.

3. **Add Your Own Content**:
   Replace the `carousel-item` contents with your own images, text, or other media.

4. **Launch the Carousel**:
   Open the HTML file in a browser, and the carousel will work as expected!

## Conclusion

This Simple JS Carousel provides a lightweight and customizable way to create carousels on your webpage. You can control the speed, enable/disable auto-sliding, and even turn off indicators depending on your preferences using data attributes.


(Jackstar-Git, September 2024)

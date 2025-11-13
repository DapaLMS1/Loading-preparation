Steriliser Check Learning Activity

Overview

This is a single-file, responsive web application designed as an interactive learning module. It presents key steps for steriliser pre-use checks using a dynamic, circular UI pattern. Users click on orbiting topic circles to display detailed information in the central main circle.

The layout is mathematically calculated in JavaScript to ensure all elements remain perfectly centered and contained within the main purple container, regardless of screen size.

Features

Interactive Orbit Layout: Small purple circles orbit a central white circle, dynamically shifting position when clicked.

Real-time Content Display: Clicking an orbiting circle instantly loads the corresponding learning text into the central display area.

Visual Feedback: The active circle enlarges and receives a green border (#7ABF49) for clear visual indication.

Enhanced Depth: Uses strong box-shadow properties to give the circles a distinct, lifted appearance.

Fully Responsive Design: The entire layout adapts to smaller screens using viewport-relative units, ensuring the interactive experience is seamless on mobile devices.

Contained Design: The layout is precisely calculated to ensure all interactive elements remain within the 650px container width.

Technology Stack

HTML5: Structure of the learning module.

CSS3: Custom styles for layout, colors, and shadows.

Tailwind CSS: Used for utility classes and foundational styling properties.

JavaScript (Vanilla JS): Handles the complex trigonometric calculations for circle positioning, click events, and state management.

Project Structure Summary

The application is contained within a single index.html file, which includes:

CSS <style> block: Defines the visual aesthetics, ensuring the large circle is a perfect 440px circle and applying the custom shadows for depth.

HTML <body>: Contains the main purple container (learning-activity-container), the central white display circle (large-circle), and a wrapper for the dynamic small circles (small-circles-wrapper).

JavaScript <script> block:

sectionsData: Contains the learning content (title and content) for the orbiting circles.

getOrbitRadius(): The critical function that calculates the distance required for the small circles to orbit the large circle and remain perfectly contained within the parent boundary.

renderCircles(): Calculates the X/Y coordinates for each circle based on its angle and the orbit radius, ensuring they are correctly positioned on the left or right arcs relative to the currently active item.

handleCircleClick(): Updates the content and triggers the renderCircles() function to animate the visual repositioning.

How to Run

This is a single-page application with no build steps or server dependencies.

Save the code as index.html.

Open the index.html file directly in any modern web browser.

The activity is ready to use.

# VNKeys JS: Vietnamese Typing Across Devices
VNKeys is a powerful and intuitive JavaScript library designed to enable users to type in Vietnamese effortlessly on any browser and device. Recognizing the challenges of inputting Vietnamese text, especially for users unfamiliar with specialized keyboards, VNKeys provides a seamless typing experience with support for multiple popular Vietnamese input methods.  Yes, it works mobile devices.

## Live Demo
Check out live demo [VNKeys.NET](https://vnkeys.net) for more details.

## Features
VNKeys supports five input modes:

1. **OFF**: Disables Vietnamese input, allowing standard typing.
2. **AUTO**: Automatically detects and applies the appropriate input method based on the user's typing patterns.
3. **VIQR**: A traditional input style using ASCII characters like `a^`, `o^`, and `dd`.
4. **VNI**: Popular among Vietnamese users, using numerical codes (e.g., `a1`, `a2`) for tone marks and accents.
5. **TELEX**: A modern and intuitive method with combinations like `aa` for â or `dd` for đ.

## Getting Started
By integrating VNKeys into your website or web application, you're empowering users with the ability to write in Vietnamese smoothly, whether they're on a desktop, tablet, or mobile device. Say goodbye to cumbersome workarounds and hello to seamless Vietnamese input with VNKeys!

## Installation

1. **Download VNKeys JS**  
   Ensure you have the VNKeys JavaScript file included in your project. Place it in an accessible location, e.g., `js/vnkeys.js`.

2. **Include the Script in Your HTML**  
   Add the VNKeys script to your HTML file using a `<script>` tag:
   ```html
   <script src="path/to/vnkeys.js"></script>
   or
   <script src="https://vnkeys.net/raw.htm?skey=vnkeys_js"></script>

   

3. **Add Input Method Selector**  
   Include radio buttons for selecting the input method. Use the `VNKeys.setMethod()` function to switch between input modes:
   ```html
   Methods: 
   <input name="vnkeys_method" type="radio" value="off" onchange="VNKeys.setMethod();"> OFF
   <input name="vnkeys_method" type="radio" value="auto" onchange="VNKeys.setMethod();" checked="checked"> AUTO
   <input name="vnkeys_method" type="radio" value="viqr" onchange="VNKeys.setMethod();"> VIQR
   <input name="vnkeys_method" type="radio" value="vni" onchange="VNKeys.setMethod();"> VNI
   <input name="vnkeys_method" type="radio" value="telex" onchange="VNKeys.setMethod();"> TELEX
   ```
   You can also use **VNKeys.setMethod("auto")**

4. **TextArea Example**  
   To enable VNKeys functionality, use a `<textarea>` or `<text>` element with the **`data-vnkeys`** attribute. This attribute activates the Vietnamese input feature.
   ```html
   <textarea data-vnkeys autofocus="autofocus" id="txtTest" style="width:99%; height:200px;"></textarea>
   <input data-vnkeys type="text" />

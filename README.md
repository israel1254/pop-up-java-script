# pop-up-java-script

A simple JavaScript project to create pop-up windows that can be used to display messages, alerts, or information to users on your website. This project demonstrates how to implement basic pop-up functionality using HTML, CSS, and JavaScript.

## Table of Contents

- [Features](#features)
- [Demo](#demo)
- [Installation](#installation)
- [Usage](#usage)
- [Customization](#customization)
- [Contributing](#contributing)
- [License](#license)

## Features

- Display a custom pop-up message to users.
- Simple and easy-to-use implementation with JavaScript.
- Options to customize the look and feel of the pop-up window.
- Dismiss or close the pop-up using a button.

## Demo

![Pop-Up JavaScript Demo](demo-screenshot.png)

## Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/israel1254/pop-up-java-script.git
    cd pop-up-java-script
    ```

2. **Open the `index.html` file in a web browser** to see the pop-up in action.

## Usage

To use the pop-up in your own project:

1. **Include the JavaScript file** in your HTML:
    ```html
    <script src="popup.js"></script>
    ```

2. **Add HTML for the pop-up container**:
    ```html
    <div id="popup" class="popup">
        <div class="popup-content">
            <span class="close-btn" onclick="closePopup()">&times;</span>
            <p>This is a pop-up message!</p>
        </div>
    </div>
    ```

3. **Initialize the pop-up** by calling `showPopup()` function in your JavaScript:
    ```javascript
    function showPopup() {
        document.getElementById("popup").style.display = "block";
    }
    function closePopup() {
        document.getElementById("popup").style.display = "none";
    }
    ```

4. **Add CSS for styling** (included in `style.css`):
    ```css
    .popup {
        display: none;
        position: fixed;
        left: 0;
        top: 0;
        width: 100%;
        height: 100%;
        background-color: rgba(0,0,0,0.5);
    }
    .popup-content {
        position: absolute;
        background-color: #fff;
        padding: 20px;
        width: 300px;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
    }
    .close-btn {
        float: right;
        cursor: pointer;
    }
    ```

## Customization

To customize the pop-up:

- Modify `popup.js` to change the behavior.
- Adjust the styles in `style.css` for colors, font sizes, animations, etc.

## Contributing

Contributions are welcome! Please fork the repository, make your changes, and submit a pull request.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/YourFeature`)
3. Commit your Changes (`git commit -m 'Add some feature'`)
4. Push to the Branch (`git push origin feature/YourFeature`)
5. Open a Pull Request

## License

Distributed under the MIT License. See `LICENSE` file for more information.

# Setting up the theme on userstyles.org

This is a fully manual process since there's no API for userstyles.org ☹️

The background images can be base64 encoded with https://www.base64-image.de/

## Style Settings

<!-- markdownlint-disable MD033 -->
<table>
    <thead>
        <tr>
            <th>Type</th>
            <th>Label</th>
            <th>Install Key</th>
            <th>Config</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Dropdown</td>
            <td>Add a background image?</td>
            <td><code>bg-choice</code></td>
            <td>
                <table>
                    <tbody>
                        <tr>
                            <td>Yes</td>
                            <td>Yes</td>
                            <td>Default</td>
                        </tr>
                        <tr>
                            <td colspan="3">
                                <pre>background-image: url(/*[[bg-image]]*/) !important;</pre>
                            </td>
                        </tr>
                        <tr>
                            <td>No</td>
                            <td>No</td>
                            <td></td>
                        </tr>
                        <tr>
                            <td colspan="3">
                                <i>leave empty</i>
                            </td>
                        </tr>
                    </tbody>
                </table>
            </td>
        </tr>
        <tr>
            <td>Image</td>
            <td>Background image</td>
            <td><code>bg-image</code></td>
            <td>
                <table>
                    <tbody>
                        <tr>
                            <td>Default</td>
                            <td>Default</td>
                            <td>Default</td>
                        </tr>
                        <tr>
                            <td colspan="3">
                                <pre>data:image/png;base64,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</pre>
                            </td>
                        </tr>
                        <tr>
                            <td>Original</td>
                            <td>Original</td>
                            <td></td>
                        </tr>
                        <tr>
                            <td colspan="3">
                                <pre>data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAGQAAABkAgMAAAANjH3HAAAACVBMVEUaGhohISElJSUh9lebAAABwElEQVR4AY3Vua3gOBgGQQXZhgKYgwHJYAA0Ksu9CAh6hxbTbvFzfx6rNEGlHY6z5KvMw4s43mN2Z5fqYLzKyrfyXhXKnKBdD9n58UWW3Vlb3mOCmWoHHZbdV5lv8t7Ver6ldsfqumVAdbblxxcZVcd7QWq2Y6VsadS4ZTzFDbFa5XivqlxVUFG1Jd6k66u8x0RIOw0cXAiNW2z58bJ5r1LTQtVVuy1x2jK+yLTlxy3v5RogszEXSB0ZF4iYWLbMMUBGPDbvpRQUVUV9kvGU6ynrIe9FOqssJcQ4oqurCjV6ytmqco4SwvGeNCoJaphwSHoK13cyuuU9ZaQI0lB1qB8zT3GL2XjKueU9pR+gH0OlqvGUzHWLQ81O0Dg95L3Uj9qxKx0pr3LdYrnlvQKlUEnV/8v4Xt6bThZROwaO5QfTUyY4GCBWu8Wf/nO4ULtj/li3mE9Z47zlx/WU94Iq7RD5XuZ6ynjIGn9yr1VhFaq2NH9s4bP4Rt5j2NFO5MBXGVsmsD5v3gslYORsd8R1i1rrIUoLKLXlvVhgKH7ApToyhk21TJhbLDvdN151vEetJtKdOtYo4SmnOvhGpjpe+xuj3X723ghdygAAAABJRU5ErkJggg==</pre>
                            </td>
                        </tr>
                    </tbody>
                </table>
            </td>
        </tr>
        <tr>
            <td>Dropdown</td>
            <td>Background image type</td>
            <td><code>bg-options</code></td>
            <td>
                <table>
                    <tbody>
                        <tr>
                            <td>Tiled</td>
                            <td>Tiled</td>
                            <td>Default</td>
                        </tr>
                        <tr>
                            <td colspan="3">
                                <pre>background-repeat: repeat !important;
background-size: auto !important;
background-position: left top !important;</pre>
                            </td>
                        </tr>
                        <tr>
                            <td>Fit window size</td>
                            <td>Fit window size</td>
                            <td></td>
                        </tr>
                        <tr>
                            <td colspan="3">
                                <pre>background-repeat: no-repeat !important;
background-size: cover !important;
background-position: center top !important;</pre>
                            </td>
                        </tr>
                    </tbody>
                </table>
            </td>
        </tr>
        <tr>
            <td>Dropdown</td>
            <td>Background image attachment</td>
            <td><code>bg-attachment</code></td>
            <td>
                <table>
                    <tbody>
                        <tr>
                            <td>Scroll</td>
                            <td>Scroll</td>
                            <td>Default</td>
                        </tr>
                        <tr>
                            <td colspan="3">
                                <pre>scroll</pre>
                            </td>
                        </tr>
                        <tr>
                            <td>Fixed</td>
                            <td>Fixed</td>
                            <td></td>
                        </tr>
                        <tr>
                            <td colspan="3">
                                <pre>fixed</pre>
                            </td>
                        </tr>
                    </tbody>
                </table>
            </td>
        </tr>
    </tbody>
</table>
<!-- markdownlint-enable MD033 -->

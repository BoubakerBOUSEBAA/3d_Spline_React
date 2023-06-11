# 3D WebSite with Spline & React JS

Hi! Here is my first code to create a web application with an animated 3D design using Spline for 3D, React and the styled-components library.

### Spline link view 3D object interactively

<https://my.spline.design/untitled-eabed8d11d1fc40dd6ca806fdfe1f111/>

### Spline visual

![Alt text](Site3DSplineReact.gif)

### Visuals Website

![Alt text](page3DSpline_React.gif)

### Dependencies

To run this code, make sure you have the following dependencies installed:

```bash
"@splinetool/react-spline"
```

enter in your terminal

```bash
yarn add @splinetool/react-spline @splinetool/runtime
```

```bash
"styled-components"
```

enter in your terminal

```bash
yarn add styled-components
```

### Make sure to install these dependencies in your project before using this code and get your own custom link on Spline to import your 3D object into the application

### How to run with yarn

```bash
yarn install
```

```bash
yarn dev
```

### How to use

Here's how you can use this code:

1. First, import the necessary components and images:

```bash
import Spline from "@splinetool/react-spline";
import styled from "styled-components";

import Logo from "./images/logo.svg";
import IconTwitter from "./images/icon-twitter.svg";
import IconYoutube from "./images/icon-youtube.svg";
import IconLapTop from "./images/icon-laptop.svg";

```

2. Export the App component as the default export:

```bash
export default function App() {
  // Your component code goes here
}

```

3. Inside the App component, use JSX to render the HTML structure:

```bash
return (
  <Wrapper>
    {/* Spline component */}
    <Spline
      className="spline"
      scene="https://prod.spline.design/34psKu9cwOYNjM2r/scene.splinecode"
    />

    {/* Content */}
    <Content>
      {/* Menu */}
      <Menu>
        {/* Logo */}
        <li>
          <img src={Logo} alt="Logo" />
        </li>
        {/* Menu items */}
        <li>
          <a href="/">Home</a>
        </li>
        <li>
          <a href="/">Download</a>
        </li>
        <li>
          <a href="/">App</a>
        </li>
        <li>
          <a href="/">Login</a>
        </li>
        <li>
          <button>Get Started</button>
        </li>
      </Menu>

      {/* Title */}
      <h1>Collaborate with Tesla</h1>

      {/* Description */}
      <p>
        Bring your team together and build your community by using our
        cross-platform app that lets you collaborate via chat, voice and by
        sharing and storing unlimited media files. A world of topics is
        waiting for you. Join the private beta.
      </p>

      {/* Download buttons */}
      <button>
        <img src={IconLapTop} alt="Download" /> Download for Mac
      </button>
      <button className="windows">
        <img src={IconLapTop} alt="Download" /> Download for Windows
      </button>
    </Content>

    {/* Social icons */}
    <Social>
      <div />
      <img src={IconTwitter} alt="Twitter" />
      <img src={IconYoutube} alt="Youtube" />
    </Social>
  </Wrapper>
);

```

4. Add the necessary CSS styles using the styled-components library:

```bash
const Wrapper = styled.div`
  font-family: "Spline Sans", sans-serif;
  font-size: 16px;
  color: white;
  position: relative;
  width: 100%;
  height: 100%;
  /* ... additional styles ... */
`;

const Content = styled.div`
  position: absolute;
  /* ... additional styles ... */
`;

const Menu = styled.ul`
  /* ... additional styles ... */
`;

const Social = styled.div`
  /* ... additional styles ... */
`;

```

5. Make sure to import the required image files so that you can use them in the code.

```text
Make sure to install the dependencies, retrieve your own custom Spline link to import your 3D object into the application, and you're good to go!
```

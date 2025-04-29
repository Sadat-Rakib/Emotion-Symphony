# Emotion-Symphony

Interactive web experience that "plays" your emotions as a cosmic particle symphony, blending 3D visuals with dynamic soundscapes for an immersive, therapeutic journey.

## Table of Contents

- [Features](#features)
- [Demo](#demo)
- [Installation](#installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [Responsive Design](#responsive-design)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

---

## Features

- **Emotion Mapping**: Select predefined emotions (Joy, Sadness, Anger, Calm) or enter a custom emotion.
- **3D Particle Visuals**: Stunning Three.js particle system whose color, speed, and background adapt to your feeling.
- **Dynamic Audio**: Real-time sound generation via the Web Audio API with frequency modulation based on emotion.
- **Therapeutic Mode**: Soothing, slow-motion animation for relaxation; toggle on/off at any time.
- **Interactive Camera**: Mouse-driven camera movement alters audio pitch and viewpoint.
- **Responsive Design**: Fluid layout and controls optimized for desktops, tablets, and mobile devices.

## Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/<Sadat-Rakib>/Emotion-Symphony.git
   cd emotion-symphony
   ```

2. **Open in browser**

   - Simply open `index.html` in your favorite browser.
   - Or serve with a static server for full Web Audio API compatibility:

     ```bash
     npx http-server .
     # then navigate to http://localhost:8080
     ```

## Usage

1. **Choose an emotion** by clicking one of the preset buttons or typing your own in the input.
2. Click **Create Symphony** to launch the visual and audio experience.
3. Move your cursor around to shift the camera and modulate sound frequency in real time.
4. Toggle **Therapeutic Mode** to slow animations and soften audio for a calming effect.
5. Resize your window or open on mobile to see the responsive layout in action.

## Configuration

You can customize emotion behavior by editing the `emotionMap` object inside the `<script>`:

```js
const emotionMap = {
  joy:     { color: 0xffff00, frequency: 440, speed: 0.05 },
  sadness: { color: 0x0000ff, frequency: 220, speed: 0.02 },
  anger:   { color: 0xff0000, frequency: 880, speed: 0.10 },
  calm:    { color: 0x00ff00, frequency: 110, speed: 0.01 },
};
```

- **color**: Hex color for particles & background.
- **frequency**: Base oscillator frequency in Hz.
- **speed**: Particle movement multiplier.

## Responsive Design

- Mobile-first layout with Tailwind CSS.
- UI panels adapt from columns to rows based on screen size.
- Controls and text scale for smaller viewports.

## Tech Stack

- **HTML5 & CSS3**
- **Tailwind CSS** – Utility-first styling
- **Three.js** – 3D particle system
- **Web Audio API** – Dynamic sound generation
- **Vanilla JavaScript (ES6)**

## Project Structure

```
emotion-symphony/
├── index.html        # Main HTML and inline JS/CSS
├── demo.gif          # Animated demo (optional)
└── README.md         # Project overview and instructions
```

## Contributing

1. Fork this repository.
2. Create your feature branch: `git checkout -b feature/my-new-feature`.
3. Commit your changes: `git commit -m 'Add some feature'`.
4. Push to the branch: `git push origin feature/my-new-feature`.
5. Submit a pull request.

Please follow the existing coding style and include clear commit messages.

## License

This project is released under the [MIT License](LICENSE).

## Contact

Mir Sadat Bin Rakib – [mirsadatbinrakib01@gmail.com](mailto:mirsadatbinrakib01@gmail.com)




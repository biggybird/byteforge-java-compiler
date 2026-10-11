# ByteForge Java Lab

A lightweight, responsive, OLED-dark online Java playground. Write Java code in the browser, provide standard input, and run it through the Wandbox compile API.

## Live Demo

**Status: Not deployed yet.**

The intended GitHub Pages address is https://biggybird.github.io/byteforge-java-compiler/ . This URL will only work after GitHub Pages is enabled and the site is published. I couldn't confirm a live deployment yet.

## Explore the projects

- **ByteForge Java Lab:** [Open this repository](https://github.com/biggybird/byteforge-java-compiler)
- **JavaLab Online Compiler:** [Open this repository](https://github.com/biggybird/javalab-online-compiler)

**JavaLab live site:** https://javalab-online-compiler.vercel.app

## Features

- OLED-friendly dark interface
- Java editor with starter code and example programs
- Standard input support
- Displays program output, compiler errors, and runtime errors
- Responsive layout for mobile and desktop
- No build step required for the static version

## Run locally

1. Download or clone this repository.
2. Open `index.html` in a modern browser.
3. Write Java code and press **Run Java**.

You can also serve the folder with any static web server.

## Deploy with GitHub Pages

1. Open the repository's **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select branch `main` and folder `/ (root)`, then save.
4. Wait for GitHub Pages to publish the site.
5. Once published, open the URL shown in GitHub Pages settings. It should normally be https://biggybird.github.io/byteforge-java-compiler/.

## Important API note

ByteForge does **not** include a Java compiler. When you click Run, your source code and standard input are sent to the third-party [Wandbox API](https://wandbox.org/), which compiles and runs it remotely. Internet access is required, and API availability, supported compiler versions, rate limits, and execution restrictions are controlled by that service. Do not submit secrets or sensitive code.

If execution fails, the cause may be API availability or a change to the compiler identifier. Check the [Wandbox website](https://wandbox.org/) and API documentation before assuming the editor itself is broken.

## Keyboard shortcut

- **Ctrl+Enter** or **⌘+Enter**: run the program.

## License

MIT. See [LICENSE](LICENSE).

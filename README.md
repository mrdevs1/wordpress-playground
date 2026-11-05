# WordPress Playground

WordPress Playground lets you run WordPress directly in your web browser without setting up a traditional hosting server or local PHP environment. It uses WebAssembly to run PHP in the browser, making it easier to test WordPress, explore plugins and themes, and experiment with different configurations.

## Overview

WordPress Playground is an open-source project maintained by the WordPress community. It provides a browser-based WordPress environment that developers, designers, students, and beginners can use without going through a full local installation process.

It also provides tools and APIs that developers can use to integrate WordPress Playground into their own applications.

## Features

- Run WordPress directly in a web browser.
- Test WordPress plugins without setting up a local server.
- Explore and customize WordPress themes.
- Select supported WordPress and PHP versions.
- Use Blueprints to configure WordPress environments.
- Save and restore supported Playground environments.
- Integrate WordPress Playground into other applications.
- Experiment with WordPress without affecting a live website.

## How It Works

WordPress Playground uses WebAssembly to run PHP inside a web browser. Since WordPress is built with PHP, this makes it possible to run a WordPress environment without relying on a traditional PHP hosting server.

The project combines WordPress, PHP WebAssembly, JavaScript, and browser APIs to provide its development environment.

## Technologies Used

- WordPress
- PHP
- WebAssembly
- JavaScript
- TypeScript
- NX
- Lerna

## Getting Started

You can try WordPress Playground without installing anything.

Visit the official website:

https://playground.wordpress.net/

Once the environment loads, you can access the WordPress dashboard, install plugins, change themes, create posts, and explore the available features.

## Running Locally

To explore the source code and work on the project locally, follow these steps.

### Requirements

- Git
- Node.js
- npm

### Clone the Repository

```bash
git clone -b trunk --single-branch --depth 1 --recurse-submodules https://github.com/WordPress/wordpress-playground.git
```

### Open the Project Directory

```bash
cd wordpress-playground
```

### Install Dependencies

```bash
npm install
```

### Start the Development Server

```bash
npm run dev
```

After the development server starts, open the following address in your browser:

```text
http://127.0.0.1:5400/
```

## Development Commands

The repository includes commands for building and maintaining different parts of the project.

### Start PHP WebAssembly CLI

```bash
npx nx start php-wasm-cli
```

### Build WordPress Releases

```bash
npx nx bundle-wordpress:all playground-wordpress-builds
```

### Recompile PHP for Web

```bash
npx nx recompile-php:all php-wasm-web
```

### Recompile PHP for Node.js

```bash
npx nx recompile-php:all php-wasm-node
```

### Build Documentation

```bash
npx nx build docs-site
```

## Project Structure

WordPress Playground is organized as a monorepo with different packages and tools.

Some of its main components include:

- WordPress: The content management system running inside Playground.
- PHP WebAssembly: Runs PHP code in supported browser environments.
- JavaScript Client: Provides tools for interacting with Playground.
- Browser Bindings: Connect the PHP runtime with browser functionality.
- Blueprints: Define and configure WordPress environments.
- Shared Packages: Provide reusable functionality across the project.

## Use Cases

WordPress Playground can be useful for:

- Learning WordPress without installing a local server.
- Testing plugins and themes.
- Experimenting with different WordPress versions.
- Developing and testing WordPress features.
- Demonstrating WordPress functionality.
- Building applications that integrate WordPress.
- Exploring WordPress development.

## Limitations

WordPress Playground is mainly designed for development, testing, learning, and experimentation. It is not intended to replace a traditional production hosting environment.

Some server-dependent services and third-party integrations may not work in the same way as they do on a regular WordPress website. Storage and persistence also depend on the selected configuration and browser capabilities.

## Contributing

WordPress Playground is an open-source project, and contributions from the community are welcome.

You can contribute by:

- Reporting bugs and issues.
- Improving existing features.
- Adding new functionality.
- Improving project documentation.
- Testing plugins and themes.
- Reviewing pull requests.

To contribute, fork the repository, create a branch for your changes, make your updates, test them, and submit a pull request.

Please review the official contribution guidelines before submitting changes.

## Useful Links

- Official Website: https://wordpress.org/playground/
- Live Demo: https://playground.wordpress.net/
- GitHub Repository: https://github.com/WordPress/wordpress-playground
- Documentation: https://developer.wordpress.org/playground/
- Developer Documentation: https://wordpress.github.io/wordpress-playground/developers/
- Contribution Guidelines: https://developer.wordpress.org/playground/handbook/contributing/

## License

WordPress Playground is distributed under the GNU General Public License, version 2 or any later version.

For more information, check the license file in the official repository.

## Repository Information

- Project Name: WordPress Playground
- Organization: WordPress
- Repository: https://github.com/WordPress/wordpress-playground
- Category: WordPress Development
- Type: Open Source Software

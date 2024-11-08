# WordCamp Larissa 2024 Repository [![Netlify Status](https://api.netlify.com/api/v1/badges/00079a62-7096-452e-8706-bbba3ebad6e6/deploy-status)](https://app.netlify.com/sites/wclagr/deploys) <!-- omit from toc -->

This repository contains resources and configuration files for WordCamp Larissa 2024, supporting various aspects of the event's online presence and community engagement.

## Table of Contents <!-- omit from toc -->

- [Project Overview](#project-overview)
- [Repository Structure](#repository-structure)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

WordCamp Larissa 2024 is a community-driven event focusing on WordPress. This repository organizes essential resources to facilitate the event's online activities, including community links, QR code redirects, and website styling.

You can read more about WordCamps in general [here](https://central.wordcamp.org/about/).

## Repository Structure

The repository is organized as follows:

```plaintext
WCLA24/
├── links/                  # Contains community links and resources for wpgreece.org/links
│   ├── css/                # CSS files specific to community links section
│   ├── fonts/              # Font files for community links section
│   ├── images/             # Image assets for community links section
│   ├── wcla2024/           # Subfolder specifically for WordCamp Larissa 2024 links
│   │   ├── css/            # CSS files specific to wcla2024 links
│   │   ├── fonts/          # Fonts used in wcla2024 links section
│   │   ├── images/         # Images used in wcla2024 links section
│   │   └── index.html      # Main HTML for wcla2024 links
│   └── index.html          # Main HTML for community links section
├── netlify-links/          # Manages QR code redirects deployed on Netlify
│   ├── _redirects          # Redirect rules for QR codes
│   ├── index.html          # Landing page for QR code redirects
│   ├── live/               # Contains the dynamic iframe rotator
│   └── qr-codes/           # Contains the QR code images
├── website-styles/         # Contains styling resources for WordCamp Larissa website
│   ├── build/              # Compiled styles ready for deployment
│   └── src/                # Source styles for customization
└──README.md                # Documentation for the repository
```

### Folder Descriptions <!-- omit from toc -->

- **links/**: Contains resources related to the WordCamp Larissa community, deployed at [wpgreece.org/links](https://wpgreece.org/links). This directory includes an `index.html` file and associated assets like `styles.css` for styling the page.

- **netlify-links/**: Manages QR code redirects, deployed via Netlify. The `_redirects` file defines URL mappings for QR codes, and the `qr-codes/` subdirectory stores the QR code images used during the event.

- **website-styles/**: Houses styling files for the [larissa.wordcamp.org](https://larissa.wordcamp.org) website. It includes compiled CSS files in the `css/` directory and source SCSS files in the `scss/` directory, facilitating customization and maintenance of the site's appearance.

- **README.md**: Provides an overview of the repository, including its structure, usage instructions, and contribution guidelines.

## Usage

Each directory serves a specific function:

- **links/**: Update the `index.html` and `styles.css` as needed to reflect current community resources. Changes are deployed to [wpgreece.org/links](https://wpgreece.org/links).

- **netlify-links/**: Modify the `_redirects` file to manage QR code destinations. Deployments are handled through Netlify.

- **website-styles/**: Edit SCSS files in the `scss/` directory to adjust the website's styling. Compile these files to CSS by using ``` npm run build ```. The compiled CSS files are stored in the `css/` directory.

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them with clear messages.
4. Push your branch to your forked repository.
5. Open a pull request to the main repository.

For major changes, please open an issue first to discuss your proposed modifications.

## License

This project is licensed under the GPL-3.0 License. See the [LICENSE](https://www.gnu.org/licenses/gpl-3.0.html) file for details.
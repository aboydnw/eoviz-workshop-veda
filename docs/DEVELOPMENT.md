This guide provides instructions for setting up and running the Next.js instance locally, as well as an overview of the development workflow.

## Prerequisites

Before you begin, ensure the following are installed on your system:

- [Node.js](https://nodejs.org/) (version specified in the [.nvmrc](../.nvmrc) file)
- [Yarn](https://yarnpkg.com/)

If you're using [`nvm`](https://github.com/nvm-sh/nvm), you can activate the required Node.js version by running:

```bash
nvm install
```

## Setting up the project

1. **Clone the repository**
    Clone the repository to your local machine:

    ```bash
    git clone https://github.com/your-org/your-repo.git
    cd your-repo
    ```

2. **Register the VEDA-UI package**
    The VEDA-UI package is now published on the public NPM registry under the @teamimpact scope. To install it, ensure your `.npmrc` or global npm configuration points to the public registry (default).

3. **Install dependencies**

    Install the project dependencies by running:

    ```sh
    yarn install
    ```

4. **Configure environment variables**

    Create a `.env.local` file in the root directory and add the necessary environment variables. Refer to the [Configuration guide](./CONFIGURATION.md) for details on required variables.

### Start the development server

To start the development server, run:

```sh
yarn dev
```

The website will then be accessible at <http://localhost:3000>.

### Building for production

To build the project for production:

```bash
yarn build
```

The output will be generated in the `.next` directory.

### Deployment

The app can be deployed to any platform supporting Node.js. Refer to your deployment platform's documentation for further instructions.


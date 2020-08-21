# editor-backend

[![Build Status](https://github.com/vega/editor-backend/workflows/Test/badge.svg)](https://github.com/vega/editor-backend/actions)

Deployed at https://editor-backend.vercel.app
~~https://vega.now.sh~~ and ~~https://vega-editor-backend.domoritz.now.sh/~~. Code is at
https://github.com/J143/editor-backend. 

## Setup Instructions

1. Clone the repository.
    ```
    $ git clone https://github.com/143/editor-backend
    ```

2. Install all dependencies.
    ```
    $ yarn install
    ```

3. Put configurations in a `.env` file in the root directory.
    ```
    $ cp .env.sample .env
    ```

4. Sample configuration of a `.env` file can be:
    ```
    # [@domoritz](https://github.com/domoritz) created this app for OAuth testing.
    # You may create [your own application](https://github.com/settings/developers).

    # GitHub OAuth app credentials
    GITHUB_CLIENT_ID=a901f0948b144d29fbdf 
    GITHUB_CLIENT_SECRET=dfdb84ff29fde4eaa160078d13e024530238ebe0

    # Session ID configuration
    SESSION_SECRET=secret
    ```

5.  Run the back-end server.
    ```
    $ yarn start
    ```

6.  Go to the home route (which usually is `http://localhost:3000/`). Otherwise
    it will be mentioned in the console where the above command is run.
    
## Documentation

Go to https://j143.github.io/editor-backend/.

## Code formatting

- Install [ESLint
  plugin](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
  for automatically handling formatting of TypeScript files.
- Install [Rewrap
  plugin](https://marketplace.visualstudio.com/items?itemName=stkb.rewrap) to
  assist formatting of markdown files. Press <kbd>Alt</kbd> + <kbd>Q</kbd> to
  limit lines at 80 characters. 
- The project uses ESLint to format the code. Run `yarn format` to fix
  formatting where it's possible to do so automatically.

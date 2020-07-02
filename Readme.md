# Testing distributable binaries for haskell-language-server

1. Ensure the URL in `.devcontainers/Dockerfile` points to the VSIX you want to test.

1. Open this folder using VS Code Remote - Containers. VS Code will build the container for you, which includes downloading the VSIX into the image.

1. Once the window has reloaded and connected to the container, open the Command Palette and choose `Extensions: Install from VSIX...`

1. Browse to `/vsix` and select the only file in the folder.

1. After a little while, VS Code will ask you to reload the window. When you do so, you'll know if the installation worked!

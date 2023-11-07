# Work in progress

## Windows Setup Steps

1. Open Powershell in Administrator mode.
2. Install neovim using chocolatey.

    ```
    choco install neovim
    ```

3. Open up nvim and figure out where your nvim config directory is.
  
    ```
    // Command
    nvim .
    
    // Neovim Command
    :echo stdpath('config')
    ```

4. Go to that directory and clone this repo there.

   ```
   cd ./path-to-folder/
   git clone <this repo>
   ```
   
5. Using nvim, open up the plugin.lua file.
   ```
   nvim ./lua/plugin.lua
   ```
6. Now install those packages using the lua packer plugin.
   ```
   // the nvim command
   :PackerSync
   // then
   :PackerInstall
   ```
7. Close the powershell and then reopen it.
8. To be continued instructions are a work in progress.

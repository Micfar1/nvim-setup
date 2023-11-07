# Work in progres

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
   git clone git@github.com:Micfar1/nvim-setup.git nvim
   ```
   
5. Using nvim, open up the plugin.lua file.

   ```
   nvim ./lua/plugin.lua
   ```

6. Now install those packages using the lua packer plugin.

   ```
   //nvim commands
   :PackerSync

   :PackerInstall
   ```

7. Close the powershell and then reopen it.
8. Go to one of your repo's and open up nvim.

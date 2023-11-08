# Windows Setup Steps

1. Install and open up [Windows Terminal](https://apps.microsoft.com/detail/windows-terminal/9N0DX20HK701?hl=en-US&gl=US).
2. Install neovim & ripgrep using chocolatey.

**Note:** ripgrep is installed for the best telescope experience. Without it, telescope attempts to search through your `node_modules` folder. 

    ```
    choco install neovim
    choco install ripgrep
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

7. From [Nerd Fonts Website](https://www.nerdfonts.com/font-downloads), download font "Sauce Code Pro".
8. In the windows explorer, go to the folder where the zip file was downloaded to.
9. Extract the zip folder and select which font you want to install, then right click that font and click "install".
10. Go to the powershell properties and under the fonts tab, select the font you installed.
11. Close the powershell and then reopen it.
12. Go to one of your repo's and open up nvim.

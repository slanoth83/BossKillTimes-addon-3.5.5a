# BossKillTimes-addon-3.5.5a

![2](https://github.com/user-attachments/assets/2ec7b4fe-fdc7-42cd-9b5b-f9d51fcf4ab1)
![1](https://github.com/user-attachments/assets/98b8283b-b254-4a29-b46b-0316c47eb525)
![pic3](https://github.com/user-attachments/assets/9a597448-5d1e-41ad-b816-0cac5ae32a91)

# Boss Kill Times (Weedsmokers Edition)

This addon displays the Top 100 fastest Naxxramas boss kills on the Warmane ladder. It specifically tracks and highlights our guild's best times and ladder rankings so we can easily see where we stand!

## Installation
1. Download the provided `.zip` file.
2. Extract the folder named **BossKillTimes** into your World of Warcraft directory: `World of Warcraft\Interface\AddOns\`.
3. Ensure the folder structure is correct. It should look like `Interface\AddOns\BossKillTimes\UI.lua`.
4. Restart your World of Warcraft client completely if it is currently running.

## How to Use
* **Minimap Button:** Click the timer icon around your minimap to open the addon interface. 
* **Locking the Button:** Right-click the minimap button to lock or unlock its position.
* **Chat Command:** Type `/bkt` in the game chat to quickly open or close the addon window.
* **Viewing Times:** Select any boss from the dropdown menu to see the Top 100 list. The Weedsmokers run will be highlighted in bright purple, and our overall best time and rank will be pinned at the top!

UPDATING. Get updated Data.lua from your friend or you need to install python and few plugins

## Advanced: How to Update the Data Yourself
WoW addons cannot read live websites while the game is open. If you want to fetch the absolute latest ladder data from Warmane yourself before a raid, you need to set up the updater script. You only need to do steps 1-3 once!

### Step 1: Install Python
1. Go to [python.org/downloads](https://www.python.org/downloads/) and download the latest version of Python for Windows.
2. Run the installer. **CRITICAL:** Before clicking "Install Now", you MUST check the box at the bottom that says **"Add python.exe to PATH"**.
3. Finish the installation.

### Step 2: Install Required Libraries
1. Open the Windows Start Menu, type `cmd`, and open the **Command Prompt**.
2. Copy and paste the following command, then press Enter:
   `pip install playwright beautifulsoup4`
3. Wait for the installation to finish.

### Step 3: Install the Browser Engine
The script needs a background browser to bypass Warmane's bot protection.
1. In the same Command Prompt window, copy and paste this command and press Enter:
   `python -m playwright install`
2. Wait for the progress bars to finish downloading the Chromium browser. Once done, you can close the Command Prompt window.

### Step 4: Running the Updater
1. Go to your WoW AddOns folder: `World of Warcraft\Interface\AddOns\BossKillTimes\`.
2. Double-click the `UpdateData.bat` file.
3. A browser window will briefly pop up and scan all 15 boss pages automatically. 
4. Once it says "Success!", the window will ask you to press any key to close.
5. In World of Warcraft, type `/reload` in the chat to load the new times!

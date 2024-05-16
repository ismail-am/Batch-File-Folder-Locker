# Batch File Folder Locker

Protect your sensitive files on Windows with this simple batch file folder locker. For a step-by-step tutorial, watch the accompanying video [here](link_to_youtube_video).

## Overview

This batch file allows you to lock a folder on your Windows computer, providing an extra layer of security for your confidential documents and personal data.

## Usage

1. **Set Password**:
   - Open the `lock_folder.bat` file with a text editor.
   - Navigate to the "UNLOCK" block (line 31).
   - Replace `"YOUR-PASSWORD"` with your chosen password inside the quotation marks.
   - Save the changes and rename the file with the `.bat` extension (if not already done).

2. **Creating a Private Folder**:
   - Double-click on the `lock_folder.bat` file.
   - This will create a private folder (named "Private") which will act as a safe.
   - Move your files to the private folder.

3. **Locking a Folder**:
   - Double-click on the `lock_folder.bat` file.
   - Follow the prompts to confirm locking the folder.
   - Once locked, the folder will be hidden and inaccessible without the password.

4. **Unlocking a Folder**:
   - Double-click on the `lock_folder.bat` file.
   - Enter the password you set earlier.
   - The folder will be restored to its original state.

<!-- This section emphasizes the importance of remembering the password and the directory location of the private folder. -->
## Important Considerations

When using this batch file to lock and hide a private folder, there are several key points to keep in mind:

### Password and Directory Location

1. **Password Security**:
   - It's crucial to remember the password you set when locking the private folder. This password is necessary for unlocking and accessing your files securely.

2. **Directory Location**:
   - Make sure to keep track of the directory where you initially activated the batch file to create the private folder. This location is where your hidden files are stored.

3. **Batch File Usage**:
   - Using the batch file in any directory will either attempt to unlock the existing private folder by prompting the user to enter the password or create a new private folder if one doesn't already exist. This ensures flexibility in managing your protected files across different directories on your system.


<!-- This section provides tips on managing the batch file and maintaining overall security awareness. -->
### Batch File Management

1. **Moving the Batch File**:
   - After locking the private folder, consider moving the batch file to a less obvious location. Storing it in a directory that you can easily remember but others might overlook can enhance security. For example, you could create a dedicated folder for system utilities or rename the batch file to something inconspicuous.

2. **Password Storage**:
   - Consider storing the password securely in a separate location, such as a text document or on your phone.

3. **Batch File Mobility**:
   - You have the flexibility to relocate the batch file to any directory within your system. Executing the batch file from various locations will generate multiple hidden folders, enabling you to arrange your concealed files as desired. Importantly, all these hidden directories will be unlockable using the same batch file and password combination initially used to create them.

4. **Deleting the Batch File**:
   - While deleting the batch file can add an extra layer of security by minimizing the risk of its discovery, exercise caution before doing so. Make sure you have a secure method for remembering the password and accessing the batch file if needed in the future. Additionally, keep in mind that the batch file can be easily found online, or a "random directory".


### Explaining Batch File Functionality

This batch file utilizes a simple yet effective technique to hide a folder by mimicking a Control Panel item. Let's break down how it accomplishes this:

#### Control Panel GUID

The key aspect of this technique is the use of a special GUID (Globally Unique Identifier), specifically `21EC2020-3AEA-1069-A2DD-08002B30309D`. This GUID is associated with the Control Panel in Windows. When appended to a folder name, it triggers a unique behavior in the operating system.

<!-- This section provides an overview of how the batch file works and its key components. -->
#### Mimicking Control Panel Item

By renaming the folder with the Control Panel GUID and setting its attributes to hidden and system, the batch file makes the folder appear as a Control Panel item to the operating system. This clever trickery allows the folder to be hidden in plain sight, providing a basic form of security through obscurity.

## Important Notes

- If you delete the original batch folder, just download the batch file, you can modify the batch file to update the password. Simply right-click on the `lock_folder.bat` file, select "Edit", and navigate to the "UNLOCK" block. You can then update the password as needed.
- Use this tool responsibly and only on folders containing sensitive information that you wish to protect.

## Original Source

This code is not my original creation. I found it on various sources online and decided to create a tutorial video and a GitHub repository, explaining it in detail, to share it here. Please refer to the original sources for any licensing information or copyright restrictions.

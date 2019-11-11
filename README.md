# windows-configuration
How to get a windows system prepared for a course environment

Add 'Open Command Window Here' to Windows 10 Context Menu. https://www.itprotoday.com/windows-10/add-open-command-window-here-windows-10-context-menu
1. Press Windows key and + R from the keyboard to open the Run command. Type regedit and then hit enter from the keyboard to open the registry.
2. Go to the following path: HKEY_CLASSES_ROOT\Directory\shell\cmd. Right-click the cmd key. Scroll to Permissions and then click it.
3. Click Advanced.
4. Click the Change link.
5. Type your user account name and click ‘Check Names’ to verify it. Click OK when you are done.
6. Check ‘Replace owner on subcontainers and objects’. Click Apply and then OK.
7. In ‘Permissions for cmd’ window, select the Administrator account. Check Allow for full control option. Click Apply and then OK.
8. Inside the cmd key (right window), right click HideBasedOnVelocityId and then click Rename.
9. Rename the DWORD from HideBasedOnVelocityId to ShowBasedOnVelocityId, then hit Enter from the keyboard.
10. You are done. When you press shift from the keyboard and then right-click on any folder, you will have the ‘Open command window here’ option on the Windows 10 Context Menu.

Remove 'Open PowerShell' from Windows 10 Context Menu. https://www.itprotoday.com/powershell/how-remove-open-powershell-windows-10-context-menu
1. Press windows key + R from the keyboard to open the run command. Type regedit and hit enter from the keyboard to open the registry.
2. Go to the following location in the registry.
3. In the registry, right-click Powershell and then click Permissions.
4. In ‘Permissions for Powershell window’, click Advanced.
5. Click the ‘Change’ link located at the top of the window.
6. Type your account name and click ‘Check Names’ to verify it. Click OK when you are done.
7. Check ‘Replace owner on subcontainers and objects’. Click Apply and then OK.
8. In ‘Permissions for Powershell window’, select administrator group. Check Allow for ‘Full Control’ option. Click Apply and then OK.
9. In Powershell subkey, create a new string value called ProgrammaticAccessOnly. (To do thisL Right-click the right window, New -> String Value. Type the name and hit Enter from the keyboard).
10. That’s it. You won’t see ‘Open PowerShell window here’ option in the context menu when you press shift and then right-click any folder.

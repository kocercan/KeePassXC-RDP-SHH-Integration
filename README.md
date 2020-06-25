# KeePassXC-RDP-SHH-Integration
1- Install "KeepassXC" and "Putty 64bit" for ssh connection.   
2- Run rdp.bat and ssh.reg in order to create uri scheme for rdp:// and ssh:// links.   
3- Create two folders in KeePassXC named RDP and SSH.   
4- Use following Auto-Type Sequence for RDP folder.   
   {USERNAME}{TAB}{PASSWORD}{ENTER}   
5- Use following Auto-Type Sequence for SSH folder.   
   {USERNAME}{ENTER}{PASSWORD}{ENTER}   
6- While creating new entries use ssh://192.168.5.244 or rdp://192.168.5.244 in URL field.   
7- Usage     
       - Open URL from KeePass    
       - When the rdp or putty window opens press CTRL+Shift+V in order to trigger Auto-Type for credentials.   
    
         
        note: You might want to clear your RDP history, it's explained well in this link.  
        http://woshub.com/how-to-clear-rdp-connections-history/


         
         Disable 
         Open RegEdit, then browse to HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Authentication\Credential Providers.  Find the one with the provider "PanV2CredProv".  Create a new DWORD in that one called "Disabled", with a value of 1.

         Vwalla.  Fixed.

         I have tested other GlobalProtect functionality, all seems to work OK still.

         Here's the article I found, and I used 'method 2' using the registry. https://social.technet.microsoft.com/Forums/office/en-US/9c23976a-3e2b-4b71-9f19-83ee3df0848b/how-to-disable-additional-credential-providers?forum=w8itprosecurity

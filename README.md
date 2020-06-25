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

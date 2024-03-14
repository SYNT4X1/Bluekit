![Bluekit Logo](../resources/bluekit.png ':size=1920')

### What is Bluekit?
Bluekit is a suite of security tools that features an array tools meant to sniff out system information such as ssh keys, listening ports, active users, users with accessible shells and more. The toolkit is meant to be used in real-time environments and was tested in the NCAE Cybergames to secure servers on simulated topology.

### Current Toolkit
- **Blueshell:** A bash-like "shell" for ssh that drops any validated user through ssh into a restricted environment.
- **Lockdown:** A system enumeration tool to list out information such as active ssh keys, listening ports, active shells, system users, and more.
- **Pingdrop:** A tool that leverages IPtables to to block and filter ICMP pings from IP addresses and subnets.
- **Quarantine:** A tool that turns on and off all network adapters on a system to effictively kill it's activity on a network.
- **LockFTP:** A tool that to audit SFTP and FTPS implementations for active users, file system access, and security.

### Installation
Bluekit has a preconfigured install script that will move the toolkit to the /opt directory on your linux machine. It will also update the environement path to include the install directory in /opt. You will need to logout of or restart the system to allow any of the path changes to function and work in your shells. If the commands are not found, please check your environments path variable ($PATH). 

#### Steps to Install
1. Download the repository
> git clone https://github.com/SYNT4X1/Bluekit.git
2. Change into the files download directory to run the install script
> cd Bluekit
3. Run the install script with sudo privileges as the modifications to path and /opt require them.
> sudo ./install
4. Logout or reboot your system
5. Check if the install was done correctly with the following
> bluekit --version

    If there is a version number dumped to the terminal, your installation is complete. Please reference the other tabs for information on implementations and configurations.
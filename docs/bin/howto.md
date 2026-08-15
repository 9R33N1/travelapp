1. Install Linux
    1. Update
    2. Set hostname  
    # sudo hostnamectl set-hostname <hostname>
    3. Configure passwordless sudo 
    # sudo visudo <username> ALL=(ALL) NOPASSWD:ALL
    4. Setting up passwordless ssh (run from Mac terminal) 
    # ssh-copy-id idgreen@<IP_ADDRESS>
    5. Install git 
    # sudo def install git
    6. Generate public/private key pair on local server # ssh-keygen
    7. Initialize local repository 
    # git init
2. Add key via GitHub Web UI: Settings (top right corner) -> SSH and GPG keys -> New SSH key
3. Clone GitHub repository 
# git clone git@github.com:9R33N1/travelapp.git

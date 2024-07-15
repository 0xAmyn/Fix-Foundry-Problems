# Fix-Foundry-Problems
Fix for some issues i have faced during installing foundry!

# Installing SOLC
Manually Download Solc

download from : 
https://binaries.soliditylang.org/linux-amd64/solc-linux-amd64-v0.8.26+commit.4a8ab42d
https://github.com/ethereum/solidity/releases

Make the binary executable:
> cd ~
> chmod +x solc-linux-amd64-v0.8.26+commit.4a8ab42d

Move the binary to /usr/local/bin or another directory in your PATH:
> sudo mv solc-linux-amd64-v0.8.26+commit.4a8ab42d /usr/local/bin/solc

Verify the installation:
> solc --version

6. Configure Foundry to Use the Local Solc
> export FOUNDRY_SOLC_VERSION=v0.8.26
> which solc
export FOUNDRY_SOLC=/usr/local/bin/solc

Or add it to your .bashrc or .bash_profile:
> echo 'export FOUNDRY_SOLC_VERSION=v0.8.26' >> ~/.bashrc
> echo 'export FOUNDRY_SOLC=/usr/local/bin/solc' >> ~/.bashrc
> source ~/.bashrc

7. Retry Compilation
> forge compile



# GEMINI_CLI_SETUP

Step-by-step installation to run gemini cli on kali linux

## STEP 1: Install Node.js 
Default kali version of node.js may be outdated install latest LTS using NodeSource
```bash 
sudo apt update 
sudo apt install -y curl
```

Installtion via NodeSource

```
curl -fsSL https://deb.nodesource.com/setup_20.x | sudo -E bash -
sudo apt install -y nodejs
```

Verify 

```
node -v
npm -v
```

## Step 2: Fix npm permissions (For Kali)

```
mkdir -p ~/.npm-global
npm config set prefix '~/.npm-global'
echo 'export PATH=$HOME/.npm-global/bin:$PATH' >> ~/.bashrc
source ~/.bashrc
```

## Step 3: Install Gemini CLI

```
npm install -g @google/gemini-cli
```

## Step 4: Login

```
gemini
```
## Quick use 
```
alias g='gemini'
```

now you can use command 'g' for quick use 

## Common Issues
“command not found”
```
export PATH=$HOME/.npm-global/bin:$PATH
```

Node version error
```
node -v
```
NODE SHOULD BE v18+ (prefer v20)



![image](https://github.com/aayush-ethclhkr/AIxCYBERSEC/Gemini_CLI)

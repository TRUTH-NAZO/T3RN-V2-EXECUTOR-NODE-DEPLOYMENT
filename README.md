# T3RN-V2-EXECUTOR-NODE-DEPLOYMENT
FIRST FUND YOUR WALLETS, NATIVE B2N AND ALL L2 CHAINS
REQUEST B2N FAUCET
https://b2n.hub.caldera.xyz/

# ALTERNATIVELY BRIDGE V1 BRN TO B2N
You will need BRN on our testnet v2 network called B2N/l2rn to bid on orders.

Bridging BRN from BRN network (v1) to arbitrum sepolia here https://brn.bridge.caldera.xyz/ 

And then bridge from arbitrum sepolia to B2N/l2rn here https://b2n.bridge.caldera.xyz/

# YOU CAN BUY SAPOLIA ETH THEN BRIDGE THEM ACROSS ALL L2S
https://www.sepoliaeth.com/buy-sepolia-eth
https://bridge.arbitrum.io/?destinationChain=arbitrum-sepolia&sourceChain=sepolia
https://testnets.superbridge.app/
https://docs.blast.io/building/bridges/testnet

# ONCE YOUR WALLET IS FUNDED THEN PROCEED TO EXECUTOR DEPLOYMENT

# CREATE SCREEN 
    
    sudo apt install git -y

    sudo apt install screen

    screen -S T3RN

    
# DEPLOY EXECUTOR

    wget https://github.com/t3rn/executor-release/releases/download/v0.58.0/executor-linux-v0.58.0.tar.gz
    tar -xvzf executor-linux-v0.58.0.tar.gz
    cd executor/executor/bin
    export ENVIRONMENT=testnet
    export LOG_LEVEL=debug
    export LOG_PRETTY=false
    export EXECUTOR_PROCESS_ORDERS=true
    export EXECUTOR_PROCESS_CLAIMS=true
    export PRIVATE_KEY_LOCAL= ADD YOUR PRIVATE KEY
    export ENABLED_NETWORKS='base-sepolia,optimism-sepolia,l2rn,unichain-sepolia,arb-sepolia'
    export EXECUTOR_PROCESS_PENDING_ORDERS_FROM_API=true
    export EXECUTOR_PROCESS_ORDERS_API_ENABLED=false
    export EXECUTOR_ENABLE_BATCH_BIDING=true
    export EXECUTOR_PROCESS_BIDS_ENABLED=true
    export EXECUTOR_MAX_L3_GAS_PRICE=1000
    export RPC_ENDPOINTS='{
    "l2rn": ["https://b2n.rpc.caldera.xyz/http"],
    "arbt": ["https://arbitrum-sepolia.drpc.org/", "https://sepolia-rollup.arbitrum.io/rpc"],
    "bast": ["https://base-sepolia-rpc.publicnode.com/", "https://base-sepolia.drpc.org/"],
    "opst": ["https://sepolia.optimism.io/", "https://optimism-sepolia.drpc.org/"],
    "unit": ["https://unichain-sepolia.drpc.org/", "https://sepolia.unichain.org/"]
    }'
    ./executor

# DETACH SCREEN 
CTRL A+D

  THATS ALL, 
  FOLLOW ME ON TWITTER FOR SWIFT UPDATES  https://x.com/Airdropbuzzz

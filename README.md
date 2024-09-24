# Pumpfun_launch_bot
This bot makes lots of profit on Pumpfun.

## Screenshots

- Make a profit

    ![image](https://github.com/user-attachments/assets/c78aebe1-7241-481a-a18d-4492e44d3f61)


- Create new SPL token on Pump.fun

    CA: [9DQZcmv3PFezYa4itDC5NCia4vWV6LKNNShNtciwqSZM](https://pump.fun/9DQZcmv3PFezYa4itDC5NCia4vWV6LKNNShNtciwqSZM)

    ![image](https://github.com/user-attachments/assets/8482390c-6923-4ac9-a633-81ec4a661350)


- Create & buy

    [3uBwg8JRepis9HuKPFUW8joavo4CdkUGmZMciY1U7CSMEjvMbMfremZmomvg6SgyNTLPzMzWg3GiWSbxcT5hybir](https://solscan.io/tx/3uBwg8JRepis9HuKPFUW8joavo4CdkUGmZMciY1U7CSMEjvMbMfremZmomvg6SgyNTLPzMzWg3GiWSbxcT5hybir)

    ![image](https://github.com/user-attachments/assets/21fd44d5-bc05-4939-b938-a6a8d4ac367d)

    
- Sell

    [mEwTYYe7vctyDRF57AY7aJUAmggbYXApGhfnEDJqrvsSgdBJyujMNBDbfHFizKBem5kRQXDMCWtcMt8VFg8ymHk](https://solscan.io/tx/mEwTYYe7vctyDRF57AY7aJUAmggbYXApGhfnEDJqrvsSgdBJyujMNBDbfHFizKBem5kRQXDMCWtcMt8VFg8ymHk)

    ![image](https://github.com/user-attachments/assets/ea8742a6-42a1-4f34-b055-56ebaa789b72)


## Features

1. Create & buy new SPL token in the same transaction on Pump.fun
2. Buy all SPL token balance as soon as possible.
3. Create new wallet and repeat the above actions.
4. Retrieve all SOL balance to the main wallet.

## How to use

1. Clone the repository

    ```sh
    git clone https://github.com/btcoin23/pumpfun_launch_bot.git
    ```

2. Install dependencies

    ```sh
    yarn install
    ```

3. Create and edit `.env` file

    ```sh
    PRIVATE_KEY=
    RPC_URL=
    ```

4. Set your configuration on `config.ts` file

    ```sh
    export const splMetaData = {
        name: '',
        symbol: '',
        url: ''
    }// SPL token metadata

    export const buyAmount = 0.1 * LAMPORTS_PER_SOL; // first buy amount
    export const jitoTip = 0.001 * LAMPORTS_PER_SOL; // jito tip 

    export const duration_buy = 10 * 1000; // 10s before new buy
    export const duration_sell = 100; // 100ms before sell
    export const max_n = 5; // do buy/sell max_n times
    ```

5. Run the bot

    ```sh
    npm start
    ```

## Author

- [Github](https://github.com/btcoin23)
- [Telegram](https://t.me/BTC0in23)

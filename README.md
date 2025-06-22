> ## Uniswap V3: A Deep-Dive Implementation
>
> This repository contains a from-scratch implementation of the core smart contracts for the Uniswap V3 protocol, built in Solidity and tested with Foundry.
>
> ### Project Goal
>
> The objective was to move beyond a surface-level understanding of DeFi's most influential Automated Market Maker (AMM). By rebuilding the core logic from first principles, I aimed to gain a fundamental mastery of **concentrated liquidity**, **tick-based accounting**, and the intricate **mathematics** that make Uniswap V3 uniquely capital-efficient. This project is a demonstration of my ability to dissect, understand, and implement complex blockchain protocols.
>
> ### Core Concepts Explored & Implemented
>
> *   **Concentrated Liquidity:** Logic for allowing liquidity providers to allocate capital within specific price ranges, rather than across the entire price curve.
> *   **Ticks and Tick Bitmaps:** Implementation of the discrete price tick system and the gas-efficient `TickBitmap` storage layout for finding active liquidity.
> *   **Swap Mathematics:** The core `swap` function, including calculating `sqrtPriceX96`, token amounts, and fees while traversing active ticks.
> *   **Liquidity Management:** Functions for minting (`mint`) and burning (`burn`) liquidity positions and correctly tracking fees owed to providers.
>
> ### Tech Stack
>
> *   **Language:** Solidity
> *   **Framework:** Foundry (Forge for testing, Cast for interaction)
> *   **Testing:** Extensive unit and integration tests to validate the mathematical correctness and contract logic against expected outcomes.

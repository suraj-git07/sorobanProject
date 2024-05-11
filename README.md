# Crowdfunding Smart Contract

This Rust smart contract, implemented on the Soroban platform running on the Stellar blockchain, facilitates crowdfunding campaigns. Donors can deposit tokens into the contract, and if the campaign reaches its target amount before the deadline, the recipient can withdraw the funds. Otherwise, donors can reclaim their tokens after the deadline.

## Functions

### `initialize`
- **Description:** Initializes the crowdfunding campaign with the recipient's address, deadline, target amount, and token contract address.
- **Parameters:**
  - `recipient`: Address of the recipient of the funds.
  - `deadline`: Unix epoch timestamp representing the deadline of the campaign.
  - `target_amount`: The amount of tokens required to reach the campaign's goal.
  - `token`: Address of the token contract used for deposits.

### `recipient`
- **Description:** Retrieves the address of the recipient of the funds.

### `deadline`
- **Description:** Retrieves the deadline timestamp of the crowdfunding campaign.

### `started`
- **Description:** Retrieves the timestamp when the crowdfunding campaign started.

### `state`
- **Description:** Retrieves the current state of the crowdfunding campaign. Possible states are Running, Success, and Expired.

### `target`
- **Description:** Retrieves the target amount of tokens for the crowdfunding campaign.

### `token`
- **Description:** Retrieves the address of the token contract used for deposits.

### `balance`
- **Description:** Retrieves the balance of tokens deposited by a specific user.
- **Parameters:**
  - `user`: Address of the user whose balance is being queried.

### `deposit`
- **Description:** Allows a user to deposit tokens into the crowdfunding campaign.
- **Parameters:**
  - `user`: Address of the user depositing tokens.
  - `amount`: The amount of tokens to deposit.

### `withdraw`
- **Description:** Allows a user to withdraw their deposited tokens after the campaign deadline, or allows the recipient to withdraw funds if the campaign is successful.
- **Parameters:**
  - `to`: Address where the withdrawn tokens should be transferred.

## Deployed Contract Addresses

- **Abundance Token Contract Address:** [CCHH2MJUUZCEFMJMRJ66U6NZ3G2R7DKCGCHI54KQIVAL4T2F76BRVQ7O]
- **Crowdfunding Contract Address:** [CCKBUEHQTWMUBTDHSVHG7YIG7HHXHCAOLASXNIQJC3JWXUKUBQ7PGYEW]


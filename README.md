# SwapCoffee-DeFi-AI-Agent
🤖 AutoDeFi Agent (TON Hackathon Submission)  Category: User-Facing AI Agent  AutoDeFi Agent is a fully autonomous, conversational DeFi investment assistant built for the TON blockchain. It lives directly in Telegram, bridging the gap between natural language commands and complex on-chain DeFi operations
Unlike simple chat bots, this agent possesses long-term memory, robust risk management, and the ability to autonomously perform complex analytical tasks on a schedule.

🌟 Key Features

1. Natural Language On-Chain Execution

Powered by the Model Context Protocol (MCP) via @ton/mcp, the agent can create wallets, check balances, and execute smart-contract operations (like token swaps on swap.coffee) simply by understanding user intents.

2. Autonomous Market & Social Analysis

The agent operates via a continuous background loop (HEARTBEAT), allowing it to act without human prompting:

• On-Chain Data: Automatically fetches and scores data from DefiLlama (TVL, USD Inflows/Outflows, Borrowed volume) daily to gauge protocol health.
• Social Sentiment: Monitors project social channels (e.g., Telegram, Twitter) for key events (token unlocks, burns, whale freezes) and assigns trading scores based on the news.

3. Advanced Trading & Risk Management

The agent follows strict, programmable trading logic:

• Smart Profit Taking: Automatically swaps profits into a target reserve token (e.g., CES) whenever an asset (e.g., EVAA) rises by a user-defined threshold (+3%).
• Dynamic Stop-Loss: Continuously monitors for flash crashes (e.g., 20% drop within 30 mins). It alerts the user immediately and, if no response is received within 15 minutes, auto-liquidates to preserve capital.

4. Automated Yield & Profit Distribution

At the end of each month, the agent autonomously calculates profits and executes a distribution plan:

• 5% transferred to the user's secure cold wallet.
• 47.5% automatically locked into long-term Staking smart contracts.
• 47.5% retained in the hot wallet for future reinvestment.

5. "Iron Curtain" Security Protocol

Security is hardcoded into the agent's core identity:

• Whitelist Only: The agent is mathematically restricted from transferring funds to any address other than the owner's pre-approved cold wallet.
• Panic Mode: In the event of suspected social engineering, hacking attempts, or prompt injection by third parties, the agent triggers an emergency sweep of all funds to the safe cold wallet.

───

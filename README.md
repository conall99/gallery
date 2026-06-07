# Derry Business Technology Strategist

Welcome to the **Derry Business Technology Strategist** repository. This specialized agent is designed to empower small-to-medium enterprises (SMEs) in the Derry and North West region by providing expert technology strategy, efficiency auditing, and sales growth advice.

## Core Specialization

This agent is specifically tailored for the **Derry local economy**. It leverages local market insights and business data to provide hyper-relevant recommendations for businesses in the region.

### Key Capabilities

- **Derry Market Insights**: Uses local business data (including regional mapping) to identify clusters, competitors, and collaboration opportunities.
- **Efficiency Auditing**: Identifies operational bottlenecks and recommends automation tools (CRMs, ERPs) to streamline workflows.
- **Sales Growth Strategy**: Provides digital marketing and e-commerce strategies optimized for the local and regional demographics.
- **Cost Reduction**: Analyzes tech stacks to identify redundant subscriptions and suggest cost-effective modern alternatives.
- **Regional Discovery**: Facilitates local business networking and competitive analysis within Derry.

## Getting Started

### Prerequisites

- An Android device to run the **Derry Strategist** app.
- A compatible on-device LLM (e.g., Gemma 3n or 4).

### Installation

1.  **Clone this repository**: `git clone https://github.com/your-repo/derry-strategist.git`
2.  **Build the Android App**: Open the `Android` directory in Android Studio and build the project. 
    *Note: Hugging Face OAuth configuration is optional and only required if you intend to download gated models.*
3.  **Sync Skills**: The specialized skills are located in `skills/built-in/business-tech-strategist`. These are automatically integrated into the app assets during the build process.

## How it Works

The agent uses a modular **Agent Skill** framework. The core logic is defined in `SKILL.md` files, which provide the LLM with the necessary persona, instructions, and local context to act as an expert strategist.

## Development

-   **Skills**: New capabilities can be added by creating folders in `skills/`.
-   **Local Data**: Regional business data is integrated through assets such as `mapDerry`.

## License

This project is licensed under the Apache License 2.0. See the [LICENSE](LICENSE) file for details.

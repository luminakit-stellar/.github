# LumenKit — Stellar Wallet Integration & Smart Contract Auditing

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Stellar](https://img.shields.io/badge/Stellar-Network-7D00FF.svg)](https://stellar.org)
[![TypeScript](https://img.shields.io/badge/TypeScript-007ACC.svg?logo=typescript&logoColor=white)](https://www.typescriptlang.org/)

LumenKit is an advanced library for integrating cryptocurrency wallets into Web3 applications on the Stellar blockchain. Inspired by [RainbowKit](https://www.rainbowkit.com/) (EVM), LumenKit brings exclusive features such as AI-powered smart contract auditing and automated security reporting.

The name **LumenKit** refers to the light of the stars (Luminance, Stellar) and the idea of a complete developer & user kit.

## 🌟 Inspiration

- **Stellar Branding**: [Stellar Brand Resources](https://www.stellar.org/brand)
- **Stellar Wallet Kit Fork**: [Fork Stellar Wallet Kit](https://github.com/Creit-Tech/Stellar-Wallets-Kit)

## 🎨 Design System

- **LumenKit Figma**: [Lumenkit Design System](https://www.figma.com/design/D3riSyCTjtEBAeg8zsJ6vm/Lumenkit?node-id=96-23&p=f&t=zWI90xiZJVLP91vN-0)

## 🔑 Core Features

### Stellar Wallet Integration
- Connect any Stellar-compatible wallet via the Stellar SDK
- Switch between multiple Stellar accounts seamlessly
- Ready-to-use UI for managing balances, sending/receiving tokens, and tracking transactions
- Native Stellar support (EVM-focused kits don't work natively on Stellar)

### AI-Powered Transaction & Smart Contract Auditing
- **Multi-Agent AI System**: LumenKit employs a sophisticated 3-agent AI architecture for comprehensive code analysis
- **Smart Code Analysis**: Before signing a transaction or smart contract, LumenKit opens a modal displaying the relevant code snippet
- **AI Interpretation**: Multi-agent AI system interprets the code and explains in plain language what the function does
- **Enhanced Security**: Helps users clearly understand what they are signing, boosting trust and security
- **Web Scraping Integration**: Automatically extracts smart contract code for analysis

### Automated Reports & Pull Requests
- **Report Button**: Available next to any audited function
- **Automated PR Generation**: When clicked, LumenKit's AI automatically generates a Pull Request on the contract's GitHub repository with:
  - The specific code snippet showing the potential issue
  - Standardized comments explaining the problem
  - User-provided description
- **CAP Implementation**: Implements CAP (Code Annotation Protocol) to standardize comments on Stellar smart contracts, fostering public collaboration and best practices

### Security & Reliability
- Fully open-source and auditable code
- Audit modal ensures every signature is transparent to the user
- GitHub integration enables traceability and community-driven improvements

## 🤖 Multi-Agent AI Architecture

LumenKit's AI auditing system is powered by **3 specialized agents** working in harmony:

### 1. **Code Analysis Agent** 🔍
- **Role**: Deep code inspection and vulnerability detection
- **Capabilities**: 
  - Static code analysis
  - Pattern recognition for common vulnerabilities
  - Security risk assessment
  - Code complexity evaluation

### 2. **Natural Language Agent** 📝
- **Role**: Translates technical code into human-readable explanations
- **Capabilities**:
  - Code-to-English translation
  - Risk level communication
  - User-friendly explanations
  - Context-aware descriptions

### 3. **Report Generation Agent** 📊
- **Role**: Creates comprehensive audit reports and automated PRs
- **Capabilities**:
  - Standardized report formatting
  - GitHub PR generation
  - CAP (Code Annotation Protocol) compliance
  - Community collaboration facilitation

### Agent Collaboration Flow
```
Code Input → Code Analysis Agent → Natural Language Agent → Report Generation Agent → User Output
     ↓              ↓                        ↓                        ↓
  Raw Code    Security Issues         Plain English          GitHub PR + Report
```

## 🌌 LumenKit vs RainbowKit (EVM)

| Feature | LumenKit | RainbowKit |
|---------|-----------|------------|
| **Blockchain Support** | Native Stellar | EVM Networks |
| **AI Auditing** | ✅ Built-in | ❌ Not available |
| **Auto PR Generation** | ✅ Yes | ❌ No |
| **CAP Standardization** | ✅ Yes | ❌ No |
| **UI Design** | RainbowKit-inspired + Stellar branding | RainbowKit design |

## 🏗️ Architecture

LumenKit ecosystem consists of three main repositories:

### 1. **Website Repository** 
- Demo site showcasing LumenKit capabilities
- Interactive examples and documentation
- Built with React + TypeScript + Vite
- **Repository**: [lumina-kit-website](https://github.com/your-username/lumina-kit-website)

### 2. **LumenKit Library**
- Core library for Stellar wallet integration
- UI components and wallet management
- TypeScript library with full type definitions
- **Repository**: [lumenkit](https://github.com/your-username/lumenkit)

### 3. **GenAI Backend**
- Multi-agent AI system for smart contract analysis
- Web scraping capabilities for code extraction
- Automated report generation and PR creation
- **Repository**: [lumina-kit-genai](https://github.com/your-username/lumina-kit-genai)

## 🚀 Quick Start

### Installation

```bash
npm install @lumenkit/stellar-wallets-kit
```

### Basic Usage

```typescript
import { LumenKitProvider, ConnectButton } from '@lumenkit/stellar-wallets-kit';

function App() {
  return (
    <LumenKitProvider>
      <ConnectButton />
    </LumenKitProvider>
  );
}
```

### AI Auditing Integration

```typescript
import { useAuditTransaction } from '@lumenkit/stellar-wallets-kit';

function TransactionComponent() {
  const { auditTransaction } = useAuditTransaction();
  
  const handleTransaction = async (transaction) => {
    const auditResult = await auditTransaction(transaction);
  };
}
```

## 🔧 Development

### Prerequisites
- Node.js 18+
- npm or pnpm
- Stellar Testnet account

### Setup

```bash
# Clone the repository
git clone https://github.com/your-username/lumina-kit.git
cd lumina-kit

# Install dependencies
npm install

# Start development server
npm run dev
```

### Repository Structure

```
LumenKit Ecosystem:
├── lumina-kit/           # Main repository (this README)
├── lumina-kit-website/   # Demo site and documentation
├── lumenkit/             # Core library
└── lumina-kit-genai/     # AI agents and web scraping
```

## 🤝 Contributing

We welcome contributions! Please see our [Contributing Guide](CONTRIBUTING.md) for details.

### Development Workflow

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add tests if applicable
5. Submit a pull request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [RainbowKit](https://www.rainbowkit.com/) for the amazing UI inspiration
- [Stellar Development Foundation](https://stellar.org) for the incredible blockchain platform
- The open-source community for continuous support and feedback

## 📞 Support

- **Documentation**: [lumina-kit.vercel.app](https://lumina-kit.vercel.app)
- **Issues**: [GitHub Issues](https://github.com/your-username/lumina-kit/issues)
- **Discord**: [Join our community](https://discord.gg/lumina-kit)

## 🔗 Related Repositories

- **[LumenKit Library](https://github.com/your-username/lumenkit)** - Core Stellar wallet integration library
- **[Website & Demo](https://github.com/your-username/lumina-kit-website)** - Interactive demo
- **[GenAI Backend](https://github.com/your-username/lumina-kit-genai)** - AI agents and smart contract analysis

---

**Built with ❤️ for the Stellar ecosystem**

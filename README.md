# 🔮 Delveil: Privacy-Preserving Link Relay Framework

> *"In the digital realm, the path matters more than the destination."*

---

## 🧿 Introduction

**Delveil** is a lightweight cryptographic relay framework designed for secure content transmission. It functions as a privacy-preserving middleware that obscures source origins while maintaining data integrity. This implementation allows for the generation of ephemeral access points to network storage assets without exposing the underlying repository infrastructure.

## 🧩 Architectural Philosophy

The project adopts principles from the **California coastal information flow paradigm**, emphasizing:

- 🌊 **Ephemeral Transmission**: Like waves on Del Mar shores, data flows leave no permanent traces
- 🏄 **Adaptive Protocols**: Responsive handling of varying content types and authentication mechanisms
- 🕸️ **Origin Obfuscation**: Complete separation between access point and source repository
- 🧠 **Stateless Operations**: No persistent storage of transient data streams

## 🔱 Core Features

- **Dynamic Link Translation**: Transforms secured repository access points into temporary public endpoints
- **Stream Relay Processing**: Direct binary stream handling without intermediate storage
- **Configurable Decay Parameters**: Time-based or use-based access expiration
- **Authentication Layer Integration**: Optional password protection for relay endpoints
- **Origin Concealment**: Complete separation between frontend and backend networks

## 🏛️ Implementation Structure

```
delveil/
├── main.py                # FastAPI implementation core
├── parsers.py             # Protocol-specific interpreters
├── config.json            # Relay configuration mapping
├── utils.py               # Utility functions including stream processing
├── templates/
│   ├── delmar.html        # Link generation interface
│   ├── encinitas.html     # File access interface
│   └── lajolla.html       # Administrative control panel
├── static/
│   ├── css/
│   │   └── style.css      # California-inspired styling
│   └── js/
│       └── script.js      # Client-side functionality
├── requirements.txt       # Dependency specifications
└── README.md              # Implementation documentation
```

## 🎭 Endpoint Masking Strategy

| Virtual Path | Function |
|--------------|----------|
| `/delmar` | Content relay initialization interface |
| `/encinitas/:code` | Ephemeral access interface |
| `/lajolla1295.html` | Administrative controls (location-obscured) |

## 🧪 Supported Protocols

The modular framework currently supports the following source protocols:

### ✅ Implemented:
- **KOD Protocol** (Fully operational)
  - Single asset relay
  - Directory structure mapping

### 🧪 Research Pipeline:
- Cloudreve Protocol (Open specification)
- Nextcloud Protocol (Self-hosted environments)

### ⚠️ Incompatible (Due to client-side validation requirements):
- Commercial repositories (Baidu, Alibaba Cloud, Tencent) with proprietary authentication mechanisms

## 🔏 Security Implementation

The security model implements several cryptographic and information theory principles:

- Non-deterministic endpoint generation
- Configurable entropy sources
- Access control parameters:
  - `max_views`: Interaction count limitations
  - `expire_at`: Temporal boundaries (UNIX timestamp)
  - `password`: Optional symmetric encryption key
- Administrative interface with enhanced authentication requirements

## 🧮 Configuration Syntax

```json
{
  "abc123": {
    "platform": "kod",
    "share_url": "https://[redacted]/#s/_Z9NwP-Q",
    "password": "y1VXy",
    "type": "file",
    "max_views": 3,
    "expire_at": 1737235200
  }
}
```

## 🏗️ Deployment Architecture

The reference implementation utilizes:

1. Ubuntu server ecosystem
2. Python 3.11+ runtime environment
3. FastAPI for asynchronous request handling
4. Playwright for protocol simulation
5. Systemd for service management and automatic startup
6. Reverse proxy configuration with TLS implementation

### Systemd Service Integration

The implementation employs systemd for service lifecycle management:

```ini
[Unit]
Description=Delveil Privacy Link Service
After=network.target

[Service]
User=www-data
WorkingDirectory=/path/to/delveil
ExecStart=/usr/bin/python3 -m uvicorn main:app --host 127.0.0.1 --port 8000
Restart=always
Environment="PLAYWRIGHT_BROWSERS_PATH=/path/to/playwright/browsers"

[Install]
WantedBy=multi-user.target
```

## 🔬 Research Applications

This implementation has potential applications in:

- Privacy-preserving content distribution
- Digital asset provenance obfuscation
- Information flow control research
- Temporary access provisioning without persistent trails
- Cross-repository content aggregation without revealing sources

## 🧭 Development Timeline

### Phase 1: Core Infrastructure (1-2 weeks)
- FastAPI framework implementation
- KOD protocol parser development
- Stream relay processing
- Base template preparation

### Phase 2: Feature Enhancement (3-4 weeks)
- Directory listing functionality
- Access control and expiration implementation
- UI design refinement
- Del Mar interface development

### Phase 3: Deployment & Testing (Week 5)
- Deployment documentation
- Security assessment
- Resource optimization
- Production testing
- Systemd service configuration

## 📋 Feature Matrix

| Feature | Status | Description |
|---------|--------|-------------|
| KOD Single File Relay | ✅ | Direct file link extraction and relay |
| KOD Directory Relay | ✅ | Directory structure navigation and access |
| Origin Domain Concealment | ✅ | Backend stream proxying |
| Configuration Management | ✅ | code → link/password/type mapping |
| Del Mar Generation Interface | ✅ | Link creation portal |
| Encinitas Access Interface | ✅ | Download interface with countdown |
| La Jolla Control Panel | ✅ | Hidden administration path |
| Deployment Integration | ✅ | Systemd and reverse proxy configuration |
| Playwright Simulation | ✅ | Automated authentication and extraction |
| Multi-platform Protocol Support | 🔜 | Planned extension to additional repositories |
| One-time Access Mechanism | 🔜 | Single-use link functionality |
| Commercial Repository Support | ❌ | Not compatible due to validation requirements |

## 🚀 Implementation Challenges

### 1. Browser Simulation Resource Management
- On-demand instance creation rather than persistent browser
- Appropriate timeout configuration to prevent resource starvation

### 2. Stream Processing
- Flow-through processing without complete file buffering
- Header preservation for seamless content type handling

### 3. Security Considerations
- Unpredictable code generation
- View limitation and expiration mechanisms

### 4. Service Management
- Systemd configuration for stability and automatic restart
- Environment variable configuration for browser path management

---

## 📜 Theoretical Foundation

Delveil draws from several disciplines in its implementation:

1. **Information Theory**: Shannon's concepts of entropy in secure transmission
2. **Cryptographic Relay Design**: Principles of data flow without source revelation
3. **California School of Digital Privacy**: Emphasizing user agency and aesthetic simplicity
4. **Ephemeral Computing**: Temporally bounded computational resources

---

*Delveil is an open implementation for academic and research purposes. The developers assume no responsibility for implementation choices in production environments.*

---
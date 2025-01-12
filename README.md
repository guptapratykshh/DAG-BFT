# DAG-BFT

A Go implementation of **FaBFT (Flexible Asynchronous BFT Protocol using DAG)** – a novel consensus algorithm designed to work efficiently in both partially synchronous and fully asynchronous networks, leveraging the BlockDAG structure to improve throughput and concurrency.

## Features

- **Flexible Consensus**: Supports both optimistic and pessimistic network assumptions, enabling clients to choose ledgers accordingly.
- **BlockDAG-based**: Organizes blocks in a DAG rather than a linear chain, improving parallelism and utilization of bandwidth.
- **Asynchronous BFT**: Removes dependency on time bounds or view change, ensuring robustness under network fluctuations.
- **Efficient CBC and GPC**: Uses Consistent Broadcast (CBC) and Global Perfect Coin (GPC) for lower latency and better randomness.

## Prerequisites

- Go 1.19 or higher
- Git

## 🛠️ Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/FaBFT-Go.git
cd FaBFT-Go
```

2. Install dependencies:
```bash
go mod download
```

## Usage

1. Build the project:
```bash
go build
```

2. Run the tests:
```bash
go test ./...
```

3. Start the node:
```bash
./fabft-go
```

## Paper

This implementation is based on the paper:

**FaBFT: Flexible Asynchronous BFT Protocol Using DAG**  
by Yu Song, Yu Long, Xian Xu, and Dawu Gu

- [ACM Digital Library](https://dl.acm.org/doi/10.1007/978-981-97-0945-8_20)

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

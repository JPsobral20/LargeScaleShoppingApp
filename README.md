# Large Scale Shopping App

The project explores distributed system concepts through a shopping cart application composed of multiple independent components, including a frontend, a proxy, and distributed workers. The components communicate using ZeroMQ, enabling distributed processing and interaction between different parts of the system.

## Architecture

The application is organized into three main components:

- **Frontend:** Handles user interaction and shopping cart operations.
- **Proxy:** Acts as an intermediary between the frontend and the distributed workers.
- **Workers:** Process requests as independent components of the distributed system.

## Technologies

- **Python 3**
- **ZeroMQ (PyZMQ)**
- **Distributed Systems Architecture**

## Getting Started

### Prerequisites

- Python 3
- pip

### Installation

Install the required dependency:

```bash
pip install pyzmq==26.0.3
```

### Running the Application

Start each component in a separate terminal, from the project root directory.

**1. Start the Proxy**

```bash
make proxy
```

**2. Start a Worker**

```bash
make worker port=6000
```

You can start additional workers using different ports.

**3. Start the Frontend**

```bash
make frontend user=alice
```

Replace `alice` with the desired username.

## Documentation

- [Project Report](doc/Relatório%20SDLE%20-%20Shopping%20Cart.pdf)
- [Video Demonstration](doc/demo_sdle_g14.mp4)

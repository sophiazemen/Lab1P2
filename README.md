# BSS Protocol for Causal Ordering using RMI

## Description
This project implements the Birman-Schiper-Stephenson (BSS) protocol for causal message ordering using Java RMI (Remote Method Invocation). It ensures that messages are delivered to processes in a causally ordered manner using vector clocks.

## Components
- **Process Interface**: Defines the methods for processes to send and deliver messages.
- **Process Implementation**: Implements the logic for handling messages and vector clocks.
- **BSSManager Interface**: Manages message passing and causal ordering.
- **BSSManager Implementation**: Enforces causal ordering using vector clocks and message queues.
- **BSSServer**: The RMI server that manages the BSSManager.
- **BSSClient**: Simulates processes sending messages through the BSSManager.

## How to Run
1. **Start the RMI Registry**: `rmiregistry`
2. **Run the Server**: `java BSSServer`
3. **Run the Client**: `java BSSClient`
4. The client will simulate processes sending messages, and the server will enforce causal ordering.

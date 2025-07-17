# java-webserver-threading

A Java-based project demonstrating three approaches to handling concurrent web requests in a simple web server: single-threaded, multithreaded, and thread pool models. This repository serves as a learning and benchmarking resource for Java web server concurrency patterns.

## Table of Contents

- [Features](#features)
- [Folder Structure](#folder-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Implementation Details](#implementation-details)
- [Contributing](#contributing)
- [License](#license)
- [Credits](#credits)

## Features

- Handles HTTP requests using various concurrency techniques
- Template implementations for benchmarking and comparison

## Folder Structure

| Folder           | Description                                |
|------------------|--------------------------------------------|
| `Multithreaded`  | Multithreaded web server implementation    |
| `SingleThreaded` | Single-threaded web server implementation  |
| `ThreadPool`     | Thread pool-based web server implementation|

## Installation

**Prerequisites:**
- Java Development Kit (JDK) 8 or newer
- Git (to clone, optional)

**Clone the repository:**
git clone https://github.com/adityabapat2003/java-webserver-threading.git
cd java-webserver-threading


**Compile the code:**
javac Multithreaded/.java
javac SingleThreaded/.java
javac ThreadPool/*.java

## Usage

Navigate to the desired implementation directory and run the server:

java Main

- The server listens on a configurable port (edit in the code as needed).
- Access `http://localhost:<port>/` in your web browser.
- Use Jmeter to test and spawn threads.
er
## Implementation Details

- **SingleThreaded:** Handles one request at a time; simple but not scalable.
- **Multithreaded:** Creates a new thread for every connection; can handle more clients but risks resource exhaustion.
- **ThreadPool:** Uses a fixed-size thread pool (via Java's `ExecutorService`), providing scalable concurrency control.

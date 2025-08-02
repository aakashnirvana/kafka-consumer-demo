# 🔄 Kafka Consumer Demo

This repository contains a **simple Java application** that demonstrates how to consume messages from an **Apache Kafka topic**. It serves as a lightweight, starter-friendly template for developers learning how to build Kafka consumer clients using the **official Kafka client library**.

---

## ✨ Features

- 📥 Basic setup for consuming Kafka messages
- ⚙️ Uses official **Apache Kafka Java client**
- 🚀 Ready-to-run **Maven project** with minimal dependencies
- 🧩 Clean, modular code for easy customization and learning

---

## 📦 Prerequisites

- ✅ Java 8 or newer  
- ✅ Maven 3.6+  
- ✅ A running Kafka cluster (local or remote)

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/aakashnirvana/kafka-consumer-demo.git
cd kafka-consumer-demo
2. Configure Kafka Connection
Update Kafka settings in src/main/resources/application.properties
or directly in your consumer class:

properties
Copy
Edit
bootstrap.servers=localhost:9092
group.id=my-consumer-group
topic.name=test-topic
3. Build the Project
bash
Copy
Edit
mvn clean install
4. Run the Kafka Consumer
bash
Copy
Edit
mvn exec:java -Dexec.mainClass="com.yourpackage.YourConsumerClass"
📝 Replace com.yourpackage.YourConsumerClass with the full path to your actual consumer class inside src/main/java.

📁 Project Structure
pgsql
Copy
Edit
kafka-consumer-demo/
├── src/
│   └── main/
│       ├── java/                  # Kafka consumer logic
│       └── resources/             # application.properties (optional)
├── pom.xml                        # Maven build configuration
├── mvnw, mvnw.cmd                 # Maven wrapper scripts
├── .gitignore
└── README.md
🧪 Usage Notes
Make sure your Kafka broker is running and the topic exists.

You can create a topic manually using Kafka CLI or configure auto-topic creation.

Watch the terminal for message output as new messages are published.

📚 Resources
Apache Kafka Official Docs

Kafka Java Client API

Kafka Quickstart Guide

📄 License
This project is open-source and available for educational and demo purposes.

Made with ☕ and Kafka by [Aakash Nirvana](https://github.com/aakashnirvana)



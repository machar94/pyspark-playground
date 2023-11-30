# Analyzing Fantasy Football Data

The purpose of this project is to investigate how the value of the fantasy football has quarterback has changed over time. The following technologies will be used / demonstrated:

**AWS Services**

* S3
* Glue
* Database and Tables
* Triggers
* Athena

**Data Formats**

* Delta Lake

## Overview

![Architecture](assets/architecture.png)

### Data Target

The data will be stored as a Delta Lake back on S3. The table within the Delta Lake will have the following schema.

```mermaid
erDiagram
    PERSON {
        int Year
        string Position
        string Player
        float FantasyPoints
    }
```

### Prerequisites

* Poetry: 

    ```shell
    curl -sSL https://install.python-poetry.org | python3 -
    ```

* Java: 

    ```shell
    sudo apt install default-jre default-jdk
    ```

* AWS Account

### Getting Started

1. Clone the repository

2. Download dependencies

    ```shell
    poetry init
    ```

# YAML Configuration Lab – Web Application Setup

## 📘 Project Overview

This project focuses on creating and validating a YAML configuration file (`app-config.yaml`) for a sample web application.  
The exercise introduces essential skills used in DevOps and cloud engineering—such as structuring configuration files, validating syntax, and converting YAML to JSON.

YAML is widely used in infrastructure-as-code (IaC), CI/CD pipelines, Kubernetes manifests, and application configurations.  
This lab builds foundational proficiency in working with configuration files safely and correctly.

***

## 🎯 Learning Objectives

*   Write well‑structured YAML configuration files
*   Understand indentation, key-value pairs, and hierarchical data
*   Validate YAML syntax using online tools
*   Convert YAML configuration to JSON

***

## 🛠 Prerequisites

Before starting, ensure you have:

*   A text editor such as **VS Code**, **Sublime Text**, or **Notepad++**
*   Basic understanding of **indentation** and **data structures**
*   (Optional) Access to YAML/JSON validators:
    *   <https://yamlvalidator.com>
    *   <https://jsonlint.com>

***

## 📂 Project Structure

    /
    ├── app-config.yaml
    ├── README.md
    └── screenshots/
          ├── yaml-validation.png
          └── yaml_to_json.png

***

## 🚀 Lab Steps

### **1. Create the YAML File**

Open your preferred code editor and create a new file named:

    app-config.yaml

***

### **2. Add Application Configuration**

Insert the following content into your YAML file:

```yaml
application:
  name: my-web-app
  version: 1.0.0
  environment: production

server:
  host: 0.0.0.0
  port: 8080

database:
  engine: mysql
  host: db.example.com
  port: 3306
  username: admin
  password: mysecurepassword
```

***

### Screenshot: Creating the YAML File

    ![editor view](screenshot/editor-view.png)

***

### **3. Validate the YAML**

Use an online validator such as:

*   <https://yamlvalidator.com>
*   <https://www.codebeautify.org/yaml-validator>

Paste your YAML content and ensure there are **no syntax errors**.

***

###  Screenshot: YAML Validation


    ![Yaml Validation](screenshots/yaml_validation.png)

***

### **4. Convert YAML to JSON**

You may use:

*   The `yq` command‑line tool
*   Online converters like <https://json2yaml.com/convert-yaml-to-json>

Example JSON output:

```json
{
  "application": {
    "name": "my-web-app",
    "version": "1.0.0",
    "environment": "production"
  },
  "server": {
    "host": "0.0.0.0",
    "port": 8080
  },
  "database": {
    "engine": "mysql",
    "host": "db.example.com",
    "port": 3306,
    "username": "admin",
    "password": "mysecurepassword"
  }
}
```

***

###  Screenshot: JSON Output


    ![yaml to json](screenshots/yaml_to_json.png)

***

## 💡 Tips & Best Practices

*   Use **consistent indentation** (2 or 4 spaces)—never use tabs!
*   Validate YAML before deploying or using in CI/CD workflows.
*   Keep sensitive values (like passwords) in **environment variables** or secrets managers—not plain YAML.

***

## ✅ Expected Outcome

By completing this lab, you should have:

*   A valid YAML configuration file
*   A JSON version of the configuration
*   A good understanding of hierarchical configuration structures
*   Screenshots documenting your workflow and validation steps

***




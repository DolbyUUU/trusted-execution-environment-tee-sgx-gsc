# Trusted Execution Environment (TEE) Setup with Intel SGX and Gramine Shielded Containers (GSC) on Ubuntu

Step-by-step instructions for setting up a **Trusted Execution Environment (TEE)** using **Intel SGX** and **Gramine Shielded Containers (GSC)** on Ubuntu. Build secure and confidential applications leveraging the power of Intel SGX and GSC.

---

## Trusted Execution Environment (TEE)

A **Trusted Execution Environment (TEE)** is a secure area within a processor that ensures sensitive data and applications are protected from unauthorized access or tampering. TEEs isolate critical execution processes from the rest of the system, enabling developers to safeguard code and data even in untrusted environments.

### Intel SGX

**Intel Software Guard Extensions (Intel SGX)** is a hardware-based technology that provides a TEE by creating isolated memory regions, called **enclaves**, within a system's RAM. These enclaves protect sensitive code and data by encrypting them and allowing only authorized processes to access them.

### Gramine Shielded Containers (GSC)

**Gramine Shielded Containers (GSC)** is an open-source framework that enables running applications inside Intel SGX enclaves using Docker containers. GSC simplifies the process of securing containerized applications by automatically creating trusted execution environments with minimal developer effort.

---

## Content

- **Installation of Intel SGX SDK and PSW**
- **Building and running Gramine Shielded Containers (GSC)**
- **Testing Intel SGX sample applications**
- **Troubleshooting common issues**

---

## Requirements

1. **Operating System**: Ubuntu 20.04 LTS or later.
2. **CPU Requirements**: A system with an Intel processor that supports **Intel SGX**.  
   - **Note**: Intel SGX is available on 6th Generation Intel Core Processors or newer.
   - **How to Check**: You can verify SGX support on your system by checking the processor specifications or using SGX detection tools.
3. **Administrative Privileges**: Root or sudo access is required.

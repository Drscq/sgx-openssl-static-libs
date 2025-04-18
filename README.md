# SGX OpenSSL Static Libraries for Linux

[![Intel SGX SSL](https://img.shields.io/badge/Intel%20SGX-SSL-blue)](https://github.com/intel/intel-sgx-ssl)
[![License](https://img.shields.io/github/license/Drscq/sgx-openssl-static-libs)](LICENSE)

This repository hosts prebuilt static libraries of OpenSSL (version 3.1.x) for use with [Intel® SGX SSL](https://github.com/intel/intel-sgx-ssl) on Linux systems. These builds are based on the [Intel SGX SSL build instructions](https://github.com/intel/intel-sgx-ssl#build-intel-sgx-ssl-package) and are intended for developers who want to link against OpenSSL inside SGX enclaves without building it from source.

---

## 🔧 Built For

- **Operating System**: Linux (tested on Ubuntu 20.04+)
- **SGX SDK**: Latest Intel SGX SDK (>= 2.21)
- **OpenSSL**: Version 3.1.x (built in 1.1.1 compatibility mode)
- **SGX SSL**: Libraries built with CVE-2020-0551 mitigations
- **Build Modes**: Release & Debug

---

## 📁 Directory Structure

```
.
├── lib64/
│   ├── libsgx_tsgxssl.a
│   ├── libsgx_usgxssl.a
│   ├── libsgx_tsgxssl_crypto.a
│   └── ...
├── include/
│   └── bn.h
    └── ...
└── README.md
```

---

## 🚀 Usage

1. Clone or download this repository

2. Link the libraries during SGX enclave build:
   
---

## 📄 License

See [License.txt](LICENSE) for license details from the upstream [Intel SGX SSL repository](https://github.com/intel/intel-sgx-ssl).

---

## 🤝 Contributing

Pull requests to update or add new versions/builds are welcome. Please ensure compatibility with the Intel SGX SDK and document build environments clearly.

---

## 🔗 References

- [Intel SGX SSL GitHub](https://github.com/intel/intel-sgx-ssl)
- [Intel SGX SDK Downloads](https://www.intel.com/content/www/us/en/developer/tools/software-guard-extensions/download.html)
- [OpenSSL Project](https://www.openssl.org)
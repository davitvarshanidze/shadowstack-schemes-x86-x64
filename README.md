# Shadow Stack Implementation for LLVM on x86_x64

This project integrates shadow stack protection into the LLVM toolchain for x86 and x86_64 targets. By instrumenting function prologues and epilogues, it securely saves and verifies return addresses using a separate shadow stack, preventing tampering by attackers. The implementation includes an LLVM IR pass (or backend patch), and a small runtime library to manage shadow stack memory. This approach provides a foundation for building control-flow integrity (CFI) mechanisms with minimal performance overhead

set(LLVM_TARGET_DEFINITIONS Passes.td)
mlir_tablegen(Passes.h.inc -gen-pass-decls -name Tensor)
add_public_tablegen_target(MLIRTensorTransformsIncGen)

add_mlir_doc(Passes -gen-pass-doc TensorPasses ./)

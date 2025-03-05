set(LLVM_LINK_COMPONENTS support)

add_clang_executable(ccelerate_code
  CcelerateCode.cpp
  )
target_link_libraries(ccelerate_code
  PRIVATE
  clangAST
  clangASTMatchers
  clangBasic
  clangFrontend
  clangSerialization
  clangTooling
  )
